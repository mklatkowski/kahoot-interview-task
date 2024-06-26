# Kahoot interview Task 2024


## Data structure - prefix tree (trie)

Trie is a type of k-ary search tree which allowes to link its nodes by individual characters. Trie's average and worst time conplexities in big O notation are O(n), so because of that, this data structure is very decent to use for this task.

## Trie's methods

### Insertion

It was decided to cast words to lowercase, after that, following characters are added (if necessary)
to the children of the previous node. At the end of insertion, the last character
of the word is marked as the end of the word.

### Searching for the words with given prefix

At the beginning, prefix is casted to lowercase. Next, given prefix in searched in the trie
If the prefix exists, algorithm looks for all suffixes with the given prefix, adds them to the prefix, and collects all these words to the result list
Otherwise, algorithm returns an empty list

## How to use the program?

For the test reason, there was created a script Program.py. In this script there is already created a Trie object, and methods which call trie's methods.
To insert words into the trie in Program.py, just call method:
>insert(word)

or if you want to add all of the words from the list:
>insert_list(word_list)

To test the algorithm, call method:
>get_words_with_prefix(prefix)

And print the result list.

If you want to use Trie structure outside Program.py, use its methods:
>trie.insert(word)

and

>trie.words_with_prefix(prefix)





