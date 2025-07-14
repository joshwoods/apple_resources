

- Natural Language
- NLGazetteer
-  write(\_:language:to:) 

Type Method

# write(\_:language:to:)

Creates a gazetteer from a set of labels for terms represented by a dictionary and saves the gazetteer to a file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func write(
    _ dictionary: [String : [String]],
    language: NLLanguage?,
    to url: URL
) throws
```

## Parameters 

`dictionary`  

The dictionary of labels and an array of terms for each label.

`language`  

The language of the text in the dictionary.

`url`  

The location in the file system to which the file should be written.

## See Also

### Creating a Gazetteer

init(contentsOf: URL) throws

Creates a Natural Language gazetteer from a model created with the Create ML framework.

init(data: Data) throws

Creates a gazetteer from a data instance.

init(dictionary: [String : [String]], language: NLLanguage?) throws

Creates a gazetteer from a set of labels for terms represented by a dictionary.

