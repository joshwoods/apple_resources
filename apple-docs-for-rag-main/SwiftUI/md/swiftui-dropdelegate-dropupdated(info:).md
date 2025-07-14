

- SwiftUI
- DropDelegate
-  dropUpdated(info:) 

Instance Method

# dropUpdated(info:)

Tells the delegate that a validated drop moved inside the modified view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
func dropUpdated(info: DropInfo) -> DropProposal?
```

**Required** Default implementation provided.

## Discussion

Use this method to return a drop proposal containing the operation the delegate intends to perform at the drop location. The default implementation of this method returns `nil`, which tells the drop to use the last valid returned value or else DropOperation.copy.

## Default Implementations

### DropDelegate Implementations

func dropUpdated(info: DropInfo) -> DropProposal?

Tells the delegate that a validated drop moved inside the modified view.

## See Also

### Receiving drop information

func dropEntered(info: DropInfo)

Tells the delegate a validated drop has entered the modified view.

**Required** Default implementation provided.

func dropExited(info: DropInfo)

Tells the delegate a validated drop operation has exited the modified view.

**Required** Default implementation provided.

func validateDrop(info: DropInfo) -> Bool

Tells the delegate that a drop containing items conforming to one of the expected types entered a view that accepts drops.

**Required** Default implementation provided.

func performDrop(info: DropInfo) -> Bool

Tells the delegate it can request the item provider data from the given information.

**Required**

