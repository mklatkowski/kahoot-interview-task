#Kahoot interview Task 2024

Trie node class with attributes:
Children - to store children nodes, keyed by characters
isFinish - to indicate if the node marks the end of a word

Main data structure - prefix tree (trie)

Insertion
Casting word to lowercase, adding following characters (if necessary)
to the children of the previous node, and marking the last character
of the word as the end of the word

Searching for the words with the given prefix
Casting prefix to lowercase and searching for the prefix in the trie

Searching for the prefix in the trie
Checking if the prefix in the trie exists
If yes, searching for all suffixes with the given prefix
else, returning an empty list

Appending all suffixes from the given node