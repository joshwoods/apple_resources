

- AppKit
- NSDocument
-  init(for:withContentsOf:ofType:) 

Initializer

# init(for:withContentsOf:ofType:)

Initializes a document with the specified contents, and places the resulting document’s file at the designated location.

macOS

``` source
@MainActor
convenience init(
    for urlOrNil: URL?,
    withContentsOf contentsURL: URL,
    ofType typeName: String
) throws
```

## Parameters 

`urlOrNil`  

The location for the document’s file. This value is `nil` for an autosaved document that the user never explicitly saved.

`contentsURL`  

The URL of the file that contains the document’s contents. When loading an autosaved document, this URL contains the location of the autosave file. The contents of this file replace the contents of the file in `absoluteDocumentURL`.

`typeName`  

The string that identifies the document type.

## Return Value

The initialized document object, or `nil` if the document could not be created.

## Discussion

The system calls this method to open a document that has an associated autosave file . You can override this method to handle any document initialization specific to autosave contents.

After reading the contents from the specified autosave file, this method updates the document’s change count using the `NSChangeReadOtherContents` change type.

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure. When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Creating a Document Object

init()

Initializes and returns an empty document object.

convenience init(contentsOf: URL, ofType: String) throws

Initializes a document located by a URL of a specified type.

convenience init(type: String) throws

Initializes a document of a specified type.

