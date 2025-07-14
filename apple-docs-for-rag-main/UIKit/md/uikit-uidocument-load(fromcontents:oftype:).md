

- UIKit
- UIDocument
-  load(fromContents:ofType:) 

Instance Method

# load(fromContents:ofType:)

Loads the document data into the app’s data model.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func load(
    fromContents contents: Any,
    ofType typeName: String?
) throws
```

## Parameters 

`contents`  

An object encapsulating the document data to load. This object is either an instance of the NSData class (for flat files) or the FileWrapper class (for file packages).

`typeName`  

The file type of the document, a Uniform Type Identifier (UTI) based on the file extension of fileURL. You can obtain the default value of the file type from the fileType property.

## Discussion

Override this method to accept and load the data for a document. After `UIDocument` reads the document data from the file located at fileURL it calls your subclass, passing the data to the subclass in this method. This method is called on the queue that the open(completionHandler:) method was called on (typically, the main queue).

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading document data

func open(completionHandler: ((Bool) -> Void)?)

Opens a document asynchronously.

func read(from: URL) throws

Reads the document data in a file at a specified location in the application sandbox.

