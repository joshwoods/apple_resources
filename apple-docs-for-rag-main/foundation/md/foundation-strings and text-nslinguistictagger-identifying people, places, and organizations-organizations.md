

- Foundation
- Strings and Text
- NSLinguisticTagger
-  Identifying People, Places, and Organizations 

Article

# Identifying People, Places, and Organizations

Use a linguistic tagger to perform named entity recognition on a string.

## Overview

Identifying named entities in natural language text can help make your app more intelligent. For example, a messaging app might look for names of people and places in text in order to display related information like contact information or directions.

The example below shows how to use NSLinguisticTagger to enumerate over natural language text and identify any named person, place, or organization.

```
let text = "The American Red Cross was established in Washington, D.C., by Clara Barton."
let tagger = NSLinguisticTagger(tagSchemes: [.nameType], options: 0)
tagger.string = text
let range = NSRange(location:0, length: text.utf16.count)
let options: NSLinguisticTagger.Options = [.omitPunctuation, .omitWhitespace, .joinNames]
let tags: [NSLinguisticTag] = [.personalName, .placeName, .organizationName]
tagger.enumerateTags(in: range, unit: .word, scheme: .nameType, options: options) { tag, tokenRange, stop in
    if let tag = tag, tags.contains(tag) {
        let name = (text as NSString).substring(with: tokenRange)
        print("\(name): \(tag)")
    }
}
```

First, an instance of NSLinguisticTagger is created, specifying nameType as the tag scheme to be used. Next, the string property of the linguistic tagger is set to the natural language text. Finally, the linguistic tagger enumerates over the entire range of the string, specifying NSLinguisticTaggerUnit.word as the tag unit and nameType as the tag scheme, omitting any punctuation or whitespace, and joining words that are part of a single name into the same token. In the enumeration block, the name type is provided by `tag`, and each word is obtained by taking a substring of the original text at `tokenRange`.

When run, this code prints out each name and its type on a new line, as shown below:

| Name | Type |
|----|----|
| The American Red Cross | organizationName |
| Washington, D.C. | placeName |
| Clara Barton | personalName |

## See Also

### Related Documentation

Tokenizing Natural Language Text

Enumerate the words in a string.

### Enumerating Linguistic Tags

Identifying Parts of Speech

Classify nouns, verbs, adjectives, and other parts of speech in a string.

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

