

- AppKit
- NSDocument
-  relinquishPresentedItem(toWriter:) 

Instance Method

# relinquishPresentedItem(toWriter:)

macOS 10.7+

``` source
nonisolated
func relinquishPresentedItem(toWriter writer: @escaping ((() -> Void)?) -> Void)
```

## See Also

### Instance Methods

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

func presentedItemDidChange()

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

func presentedItemDidGain(NSFileVersion)

func presentedItemDidLose(NSFileVersion)

func presentedItemDidMove(to: URL)

func presentedItemDidResolveConflict(NSFileVersion)

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

