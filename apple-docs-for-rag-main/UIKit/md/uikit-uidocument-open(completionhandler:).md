

- UIKit
- UIDocument
-  open(completionHandler:) 

Instance Method

# open(completionHandler:)

Opens a document asynchronously.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func open(completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func open() async -> Bool
```

## Parameters 

`completionHandler`  

A block with code to execute after the open operation concludes. The block returns no value and has one parameter:

`success`  
true if the open operation succeeds, otherwise false.

The block is invoked on the main queue.

## Discussion

Call this method to begin the sequence of method calls that opens and reads a document asynchronously. The method obtains the file-system location of the document from the fileURL property. After the open operation concludes, the code in `completionHandler` is executed.

You can override this method if you want custom document-opening behavior, but if you do it’s recommended that you call the superclass implementation first (`super`). If you don’t call `super`, you should use the NSFileCoordinator class to implement coordinated reading. The default implementation calls performAsynchronousFileAccess(_:) to schedule the document-reading work for execution on a background queue and then, from the dispatched block, performs file coordination. The queued task then calls read(from:).

## See Also

### Reading document data

func load(fromContents: Any, ofType: String?) throws

Loads the document data into the app’s data model.

func read(from: URL) throws

Reads the document data in a file at a specified location in the application sandbox.

