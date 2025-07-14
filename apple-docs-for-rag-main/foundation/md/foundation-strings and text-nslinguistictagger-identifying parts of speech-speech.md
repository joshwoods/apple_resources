

- Foundation
- Strings and Text
- NSLinguisticTagger
-  Identifying Parts of Speech 

Article

# Identifying Parts of Speech

Classify nouns, verbs, adjectives, and other parts of speech in a string.

## Overview

Identifying the parts of speech for words in natural language text can help your program understand the meaning of sentences. For example, given the transcription of a request spoken by the user, you might determine general intent by looking at only the nouns and verbs.

The example below shows how to use NSLinguisticTagger to enumerate over natural language text and identify the part of speech for each word.

```
let text = "The ripe taste of cheese improves with age."
let tagger = NSLinguisticTagger(tagSchemes: [.lexicalClass], options: 0)
tagger.string = text
let range = NSRange(location: 0, length: text.utf16.count)
let options: NSLinguisticTagger.Options = [.omitPunctuation, .omitWhitespace]
tagger.enumerateTags(in: range, unit: .word, scheme: .lexicalClass, options: options) { tag, tokenRange, _ in
    if let tag = tag {
        let word = (text as NSString).substring(with: tokenRange)
        print("\(word): \(tag)")
    }
}
```

First, an instance of NSLinguisticTagger is created, specifying lexicalClass as the tag scheme to be used. Next, the string property of the linguistic tagger is set to the natural language text. Finally, the linguistic tagger enumerates over the entire range of the string, specifying NSLinguisticTaggerUnit.word as the tag unit and lexicalClass as the tag scheme, and omitting any punctuation or whitespace. In the enumeration block, the part of speech is provided by `tag`, and each word is obtained by taking a substring of the original text at `tokenRange`.

When run, this code prints out each word and its part of speech on a new line, as shown below:

| Word | Part of speech |
|----|----|
| The | determiner |
| ripe | adjective |
| taste | noun |
| of | preposition |
| cheese | noun |
| improves | verb |
| with | preposition |
| age | noun |

## See Also

### Related Documentation

Tokenizing Natural Language Text

Enumerate the words in a string.

### Enumerating Linguistic Tags

Identifying People, Places, and Organizations

Use a linguistic tagger to perform named entity recognition on a string.

func enumerateTags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string for a particular unit and calls the specified block for each tag.

Deprecated

func enumerateTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string and calls the specified block for each tag.

Deprecated

class func enumerateTags(for: String, range: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given string and calls the specified block for each tag.

Deprecated

struct Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

