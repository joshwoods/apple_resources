

- AppKit
- NSDocument
-  accommodatePresentedItemDeletion(completionHandler:) 

Instance Method

# accommodatePresentedItemDeletion(completionHandler:)

macOS 10.7+

``` source
nonisolated
func accommodatePresentedItemDeletion(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
nonisolated
func accommodatePresentedItemDeletion() async throws
```

## See Also

### Instance Methods

func presentedItemDidChange()

func presentedItemDidChangeUbiquityAttributes(Set&lt;URLResourceKey>)

func presentedItemDidGain(NSFileVersion)

func presentedItemDidLose(NSFileVersion)

func presentedItemDidMove(to: URL)

func presentedItemDidResolveConflict(NSFileVersion)

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

