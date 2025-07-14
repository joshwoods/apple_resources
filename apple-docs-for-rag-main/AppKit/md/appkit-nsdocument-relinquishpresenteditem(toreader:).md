

- AppKit
- NSDocument
-  relinquishPresentedItem(toReader:) 

Instance Method

# relinquishPresentedItem(toReader:)

macOS 10.7+

``` source
nonisolated
func relinquishPresentedItem(toReader reader: @escaping ((() -> Void)?) -> Void)
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

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

