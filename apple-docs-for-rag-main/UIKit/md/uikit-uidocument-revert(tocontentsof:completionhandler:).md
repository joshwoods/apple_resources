

- UIKit
- UIDocument
-  revert(toContentsOf:completionHandler:) 

Instance Method

# revert(toContentsOf:completionHandler:)

Reverts a document to the most recent document data stored on-disk.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func revert(
    toContentsOf url: URL,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
@MainActor
func revert(toContentsOf url: URL) async -> Bool
```

## Parameters 

`url`  

A file URL locating the most recent version of the document file in the application’s sandbox.

`completionHandler`  

A block with code to execute after the reversion operation concludes. The block returns no value and has one parameter:

`success`  
true if the reversion operation succeeds, otherwise false.

The block is invoked on the main queue.

## Discussion

You call this method to discard all unsaved document modifications and replace the document’s contents by reading the file or file package located by `url`. The default implementation brackets the reversion operation between disableEditing() and enableEditing()because the document shouldn’t accept user changes during this period. Subclasses that override this method must call the superclass implementation (`super`) or use the NSFileCoordinator class to initiate a coordinated read.

