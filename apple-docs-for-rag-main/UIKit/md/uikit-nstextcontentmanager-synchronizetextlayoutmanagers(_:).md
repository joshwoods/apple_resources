

- UIKit
- NSTextContentManager
-  synchronizeTextLayoutManagers(\_:) 

Instance Method

# synchronizeTextLayoutManagers(\_:)

Synchronizes changes to all nonprimary text layout managers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func synchronizeTextLayoutManagers(_ completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func synchronizeTextLayoutManagers() async throws
```

## Parameters 

`completionHandler`  

A completion handler that runs on success, or to handle error conditions.

## Discussion

If `completionHandler` is `nil`, this method performs the operation synchronously. The framework passes any error to the `completionHandler`. The method blocks (or fails, if synchronous) when there’s an active transaction.

## See Also

### Working with layout managers

var primaryTextLayoutManager: NSTextLayoutManager?

The primary text layout manager for this content.

var textLayoutManagers: [NSTextLayoutManager]

The array of text layout managers associated with this text content manager.

var automaticallySynchronizesTextLayoutManagers: Bool

Determines if the framework should automatically synchronize all text layout managers when exiting an editing transaction.

func addTextLayoutManager(NSTextLayoutManager)

Adds the layout manager you provide to the list of layout managers.

func removeTextLayoutManager(NSTextLayoutManager)

Removes the layout manager you specifiy from the list of layout managers.

