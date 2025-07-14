

- Natural Language
- NLGazetteer
-  init(data:) 

Initializer

# init(data:)

Creates a gazetteer from a data instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(data: Data) throws
```

## Parameters 

`data`  

A gazetteer contained in a data instance.

## See Also

### Creating a Gazetteer

init(contentsOf: URL) throws

Creates a Natural Language gazetteer from a model created with the Create ML framework.

init(dictionary: [String : [String]], language: NLLanguage?) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary.

class func write([String : [String]], language: NLLanguage?, to: URL) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary and saves the gazetteer to a file.

