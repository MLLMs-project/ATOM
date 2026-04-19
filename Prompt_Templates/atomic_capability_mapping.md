#### Instructions
You are given an input JSON list called "atom", where each element contains a criterion,
ground_truth, and weight. Your task is to map each criterion to exactly one leaf node in
the capability tree provided below. Then output a JSON list in which each original element from
"atom" is copied verbatim, with the only modification being the addition of a new field "cap",
whose value is one leaf-node path in the format:
"<Level1><Level2><Level3>"
For example: "<Knowledge><Knowledge Retrieval><Table Lookup>".

#### Capability Tree
{Tree}

#### Output Format
Strictly output:
[
  {{
    ... original atom element fields ...,
    "cap": "one selected leaf node path"
  }},
  ...
]

#### Input Data
<question> {prompt_text} </question>
<atom> {atom} </atom>