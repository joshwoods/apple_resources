

- Core Services
- Search Kit
-  Text Analysis Keys 

API Collection

# Text Analysis Keys

Each of these constants is an optional key in a Search Kit index’s text analysis properties dictionary. The constant descriptions describe the corresponding values for each of these keys. These keys are declared in the `Analysis.h` header file.

## Topics

### Constants

let kSKMinTermLength: CFString!

The minimum term length to index. Specified as a CFNumber object. If this optional key is not present, Search Kit indexing defaults to a minimum term length of 1.

let kSKStopWords: CFString!

A set of stopwords—words not to index. Specified as a CFSet object. There is no default stopword list. You must supply your own.

let kSKSubstitutions: CFString!

A dictionary of term substitutions—terms that differ in their character strings but that match during a search. Specified as a CFDictionary object.

let kSKMaximumTerms: CFString!

let kSKProximityIndexing: CFString!

let kSKTermChars: CFString!

let kSKStartTermChars: CFString!

let kSKEndTermChars: CFString!

