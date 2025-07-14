

- SwiftUI
- DropDelegate
-  dropEntered(info:) 

Instance Method

# dropEntered(info:)

Tells the delegate a validated drop has entered the modified view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
func dropEntered(info: DropInfo)
```

**Required** Default implementation provided.

## Discussion

The default implementation does nothing.

## Default Implementations

### DropDelegate Implementations

func dropEntered(info: DropInfo)

Tells the delegate a validated drop has entered the modified view.

## See Also

### Receiving drop information

func dropExited(info: DropInfo)

Tells the delegate a validated drop operation has exited the modified view.

**Required** Default implementation provided.

func dropUpdated(info: DropInfo) -> DropProposal?

Tells the delegate that a validated drop moved inside the modified view.

**Required** Default implementation provided.

func validateDrop(info: DropInfo) -> Bool

Tells the delegate that a drop containing items conforming to one of the expected types entered a view that accepts drops.

**Required** Default implementation provided.

func performDrop(info: DropInfo) -> Bool

Tells the delegate it can request the item provider data from the given information.

**Required**

