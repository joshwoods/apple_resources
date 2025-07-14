

- AppKit
- NSDocument
-  presentedItemDidGain(\_:) 

Instance Method

# presentedItemDidGain(\_:)

macOS 10.7+

``` source
nonisolated
func presentedItemDidGain(_ version: NSFileVersion)
```

## See Also

### Instance Methods

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

func presentedItemDidChange()

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

func presentedItemDidLose(NSFileVersion)

func presentedItemDidMove(to: URL)

func presentedItemDidResolveConflict(NSFileVersion)

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

