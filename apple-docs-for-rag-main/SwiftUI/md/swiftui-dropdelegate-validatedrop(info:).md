

- SwiftUI
- DropDelegate
-  validateDrop(info:) 

Instance Method

# validateDrop(info:)

Tells the delegate that a drop containing items conforming to one of the expected types entered a view that accepts drops.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
func validateDrop(info: DropInfo) -> Bool
```

**Required** Default implementation provided.

## Discussion

Specify the expected types when you apply the drop modifier to the view. The default implementation returns `true`.

## Default Implementations

### DropDelegate Implementations

func validateDrop(info: DropInfo) -> Bool

Tells the delegate that a drop containing items conforming to one of the expected types entered a view that accepts drops.

## See Also

### Receiving drop information

func dropEntered(info: DropInfo)

Tells the delegate a validated drop has entered the modified view.

**Required** Default implementation provided.

func dropExited(info: DropInfo)

Tells the delegate a validated drop operation has exited the modified view.

**Required** Default implementation provided.

func dropUpdated(info: DropInfo) -> DropProposal?

Tells the delegate that a validated drop moved inside the modified view.

**Required** Default implementation provided.

func performDrop(info: DropInfo) -> Bool

Tells the delegate it can request the item provider data from the given information.

**Required**

