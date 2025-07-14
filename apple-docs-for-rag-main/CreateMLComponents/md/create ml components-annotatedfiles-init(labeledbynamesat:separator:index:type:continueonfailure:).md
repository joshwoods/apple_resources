

- Create ML Components
- AnnotatedFiles
-  init(labeledByNamesAt:separator:index:type:continueOnFailure:) 

Initializer

# init(labeledByNamesAt:separator:index:type:continueOnFailure:)

Reads training examples from a directory containing files having their labels in the name. The name can contain multiple words separated by a `separator`. So the `index` tells the position of the label in the file name. Files with incorrect name format are ignored.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    labeledByNamesAt url: URL,
    separator: Character = ".",
    index: Int = 0,
    type: UTType,
    continueOnFailure: Bool = false
) throws
```

## Parameters 

`url`  

URL of directory containing the files.

`separator`  

The separator used in the name. Default value is “.”

`index`  

Index of the label in the file name. Default value is 0.

`type`  

Type of files.

`continueOnFailure`  

A Boolean value indicating whether to continue reading files after encountering a file that is not readable. The default value is `false`.

## Discussion

Take for example this directory structure:

```
/
    fold1-foo-file1.png
    fold1-foo-file2.png
    fold2-foo-file3.png
    fold1-bar-file4.png
    fold1-bar-file5.png
    fold2-bar-file6.png
```

When we specify separator as “-” and index as 1, it would produce two labels (foo and bar) with three URLs each.

## See Also

### Creating the feature

init(labeledBySubdirectoryNamesAt: URL, type: UTType, continueOnFailure: Bool) throws

Reads training examples from a directory containing files in labeled sub-directories.

