# defining-tools
defining physical making tools as structured data using JSON and JSON schema

"tool-family.json"

>Document used to define high level categories or "families" of tool e.g. hand tools.

"tool-type.json"

>Document used to define types of tools that fall within tool families e.g. Hex key which fall under the tool family hand tools. "tool-type.json references "tool-family.json".

"tool-product.json"

>Contains all variations available on a type of tool such as a Hex key. "tool-product.json" references many documents including units, dimensions, materials and standards. Documents referenced as options on which a "tool-object.json" document can match.

"tool-object.json"

>Document refers to specific tool available to buy through a supplier. A hardware-object will match certain options within "tool-product.json" enabling specs to be described seperatly to solutions. The exact solution or "tool-object" can be chosen by a maker based on the spec described through selections made in "tool-product.json". Quantified config doc. needed to list selections made in "tool-product.json" enabling match to "tool-object.json" docs. Many matches expected in most cases.

"tool-set.json"

>Document contains set of configured "tool-product.json" docs enabling tools to be group based on tasks e.g. Opendesk assembly tool set containing clamps, mallet, hex key. Document must not contain "tool-object.json" docs or exact solutions will be referenced rather than specifications.
