

- AppKit
- NSDocument
-  presentedItemDidChange() 

Instance Method

# presentedItemDidChange()

macOS 10.7+

``` source
nonisolated
func presentedItemDidChange()
```

## See Also

### Instance Methods

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

func presentedItemDidGain(NSFileVersion)

func presentedItemDidLose(NSFileVersion)

func presentedItemDidMove(to: URL)

func presentedItemDidResolveConflict(NSFileVersion)

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

