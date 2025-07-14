

- Natural Language
- NLGazetteer
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Creates a Natural Language gazetteer from a model created with the Create ML framework.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(contentsOf url: URL) throws
```

## Parameters 

`url`  

The location of the .`mlmodel` file that contains a gazetteer.

## Discussion

Use this initializer to create an NLGazetteer from an `.mlmodel` file saved by MLGazetteer in the `Create ML` framework.

## See Also

### Creating a Gazetteer

init(data: Data) throws

Creates a gazetteer from a data instance.

init(dictionary: [String : [String]], language: NLLanguage?) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary.

class func write([String : [String]], language: NLLanguage?, to: URL) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary and saves the gazetteer to a file.

