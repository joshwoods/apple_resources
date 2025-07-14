

- Natural Language
- NLGazetteer
-  init(dictionary:language:) 

Initializer

# init(dictionary:language:)

Creates a gazetteer from a set of labels for terms represented by a dictionary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    dictionary: [String : [String]],
    language: NLLanguage?
) throws
```

## Parameters 

`dictionary`  

The dictionary of labels and an array of terms for each label.

`language`  

The language of the text in the dictionary.

## See Also

### Creating a Gazetteer

init(contentsOf: URL) throws

Creates a Natural Language gazetteer from a model created with the Create ML framework.

init(data: Data) throws

Creates a gazetteer from a data instance.

class func write([String : [String]], language: NLLanguage?, to: URL) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary and saves the gazetteer to a file.

