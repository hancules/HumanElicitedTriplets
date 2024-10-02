# HumanElicitedTriplets
The triplets that are elicited from language users.
Information contained is:
-  `target, elicited_relation, relatum` form a elicited triple.
-  `documented_relation` is the relation in which `(target, relatum)` is documented in WordNet. It could be either hypernymy, hyponymy, holonymy, meronymy, antonymy, and synonymy. If `(target, relatum)` is not documented in WordNet as the six relations, `documented_relation` is `None`.
-   `status` describeds the alignment between `documented_relation` and `elicitation_relation`. It have three possible values:
    - `Matched`: `documented_relation` and `elicitation_relation` are the same,
    - `Mismatched`: `documented_relation` and `elicitation_relation` are the different, and
    - `Missing`: `documented_relation` is `None`
-  `kind` refers to whther `(target, relatum)` are all abstract or physical words.
-  `prob` takes a real value, showing the elicitation frequency of the given triplet.
-  `hapax` takes a binary value, showing whether the given triplet is elicited only once.
-  `min_distance`` is the length of the shortest path that connects `target` and `relatum` in WordNet hierarchy.
