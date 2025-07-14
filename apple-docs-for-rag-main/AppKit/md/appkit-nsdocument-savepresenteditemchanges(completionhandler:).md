

- AppKit
- NSDocument
-  savePresentedItemChanges(completionHandler:) 

Instance Method

# savePresentedItemChanges(completionHandler:)

macOS 10.7+

``` source
nonisolated
func savePresentedItemChanges(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
nonisolated
func savePresentedItemChanges() async throws
```

## Discussion

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

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

