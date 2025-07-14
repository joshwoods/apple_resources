

- UIKit
- UIDocument
-  read(from:) 

Instance Method

# read(from:)

Reads the document data in a file at a specified location in the application sandbox.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func read(from url: URL) throws
```

## Parameters 

`url`  

A file URL that identifies the location of the document file in the application sandbox. This file URL is typically the one returned by the fileURL property.

## Discussion

Typical UIDocument subclasses shouldn’t need to call this method directly, especially if the entire file is read at once. The default implementation calls load(fromContents:ofType:) on the queue on which open(completionHandler:) was called to provide the `UIDocument` subclass with the document data object.

Subclasses that want more control over the reading of the document file—for example, that want to read a large document file incrementally—can override this method. It isn’t necessary for these subclasses to call the superclass implementation (`super`).

Handling Errors in Swift

In Swift, this method is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

When overriding this method, use the `throw` statement to throw an `NSError`, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Reading document data

func open(completionHandler: ((Bool) -> Void)?)

Opens a document asynchronously.

func load(fromContents: Any, ofType: String?) throws

Loads the document data into the app’s data model.

