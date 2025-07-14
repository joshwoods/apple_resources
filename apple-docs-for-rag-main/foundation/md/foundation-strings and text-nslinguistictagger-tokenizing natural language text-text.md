

- Foundation
- Strings and Text
- NSLinguisticTagger
-  Tokenizing Natural Language Text 

Article

# Tokenizing Natural Language Text

Enumerate the words in a string.

## Overview

When you work with natural language text, it’s often useful to tokenize the text into individual words. Using NSLinguisticTagger to enumerate words, rather than simply splitting components by whitespace, ensures correct behavior in multiple scripts and languages. For example, neither Chinese nor Japanese uses spaces to delimit words.

The example and accompanying steps below show how you use NSLinguisticTagger to enumerate over the words in natural language text.

```
let text = """
All human beings are born free and equal in dignity and rights.
They are endowed with reason and conscience and should act towards one another in a spirit of brotherhood.
"""

let tagger = NSLinguisticTagger(tagSchemes: [.tokenType], options: 0)
tagger.string = text

let range = NSRange(location: 0, length: text.utf16.count)
let options: NSLinguisticTagger.Options = [.omitPunctuation, .omitWhitespace]
tagger.enumerateTags(in: range, unit: .word, scheme: .tokenType, options: options) { _, tokenRange, _ in
    let word = (text as NSString).substring(with: tokenRange)
    print(word)
}
```

1.  Create an instance of NSLinguisticTagger, specifying tokenType as the tag scheme to be used.

2.  Set the string property of the linguistic tagger to the natural language text.

3.  Enumerate over the entire range of the string by calling the enumerateTags(in:unit:scheme:options:using:) method, specifying NSLinguisticTaggerUnit.word as the tag unit and tokenType as the tag scheme to enumerate, and omitting any punctuation or whitespace.

4.  In the enumeration block, take a substring of the original text at `tokenRange` to obtain each word.

5.  Run this code to print out each word in `text` on a new line.

## See Also

### Related Documentation

Identifying Parts of Speech

Classify nouns, verbs, adjectives, and other parts of speech in a string.

Identifying People, Places, and Organizations

Use a linguistic tagger to perform named entity recognition on a string.

### First Steps

init(tagSchemes: [NSLinguisticTagScheme], options: Int)

Creates a linguistic tagger instance using the specified tag schemes and options.

Deprecated

var string: String?

The string being analyzed by the linguistic tagger.

Deprecated

