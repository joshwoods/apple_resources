

- UIKit
- UIDocument
-  performAsynchronousFileAccess(\_:) 

Instance Method

# performAsynchronousFileAccess(\_:)

Schedules a document-reading or document-writing operation on a concurrent background queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func performAsynchronousFileAccess(_ block: @escaping () -> Void)
```

## Parameters 

`block`  

A block that’s invoked as the task to execute on the background queue. The block returns no value and takes no parameters.

## Discussion

A typical UIDocument subclass — one that overrides contents(forType:) and load(fromContents:ofType:) — doesn’t need to call this method.

The default implementations of save(to:for:completionHandler:) and open(completionHandler:) call this method to serialize file access. If you override these methods and don’t call `super`, you should call this method to serialize file access on a background queue. If you directly call the read(from:) method, you should wrap that call in the block passed into performAsynchronousFileAccess(_:).

