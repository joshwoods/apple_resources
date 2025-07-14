

- SwiftUI
- DropDelegate
-  performDrop(info:) 

Instance Method

# performDrop(info:)

Tells the delegate it can request the item provider data from the given information.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
func performDrop(info: DropInfo) -> Bool
```

**Required**

## Return Value

A Boolean that is `true` if the drop was successful, `false` otherwise.

## Discussion

Incorporate the received data into your app’s data model as appropriate.

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

func validateDrop(info: DropInfo) -> Bool

Tells the delegate that a drop containing items conforming to one of the expected types entered a view that accepts drops.

**Required** Default implementation provided.

