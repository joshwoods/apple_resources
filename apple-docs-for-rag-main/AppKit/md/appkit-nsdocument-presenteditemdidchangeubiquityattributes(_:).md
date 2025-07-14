

- AppKit
- NSDocument
-  presentedItemDidChangeUbiquityAttributes(\_:) 

Instance Method

# presentedItemDidChangeUbiquityAttributes(\_:)

macOS 10.13+

``` source
nonisolated
func presentedItemDidChangeUbiquityAttributes(_ attributes: Set)
```

## See Also

### Instance Methods

func accommodatePresentedItemDeletion(completionHandler: ((any Error)?) -> Void)

func presentedItemDidChange()

func presentedItemDidGain(NSFileVersion)

func presentedItemDidLose(NSFileVersion)

func presentedItemDidMove(to: URL)

func presentedItemDidResolveConflict(NSFileVersion)

func relinquishPresentedItem(toReader: ((() -> Void)?) -> Void)

func relinquishPresentedItem(toWriter: ((() -> Void)?) -> Void)

func savePresentedItemChanges(completionHandler: ((any Error)?) -> Void)

