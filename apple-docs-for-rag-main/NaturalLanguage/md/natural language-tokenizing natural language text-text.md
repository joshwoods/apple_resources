

- Natural Language
-  Tokenizing natural language text 

Article

# Tokenizing natural language text

Enumerate the words in a string.

## Overview

When you work with natural language text, it’s often useful to tokenize the text into individual words. Using NLTokenizer to enumerate words, rather than simply splitting components by whitespace, ensures correct behavior in multiple scripts and languages. For example, neither Chinese nor Japanese uses spaces to delimit words.

The example and accompanying steps below show how you use NLTokenizer to enumerate over the words in natural language text.

```
let text = """
All human beings are born free and equal in dignity and rights.
They are endowed with reason and conscience and should act towards one another in a spirit of brotherhood.
"""

let tokenizer = NLTokenizer(unit: .word)
tokenizer.string = text

tokenizer.enumerateTokens(in: text.startIndex..

1.  Create an instance of NLTokenizer, specifying NLTokenUnit.word as the unit to tokenize.

2.  Set the string property of the tokenizer to the natural language text.

3.  Enumerate over the entire range of the string by calling the enumerateTokensInRange:usingBlock: method, specifying the entire range of the string to process.

4.  In the enumeration block, take a substring of the original text at `tokenRange` to obtain each word.

5.  Run this code to print out each word in text on a new line.

## See Also

### Tokenization

class NLTokenizer

A tokenizer that segments natural language text into semantic units.

