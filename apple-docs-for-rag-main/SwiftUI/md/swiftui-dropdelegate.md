

- SwiftUI
-  DropDelegate 

Protocol

# DropDelegate

An interface that you implement to interact with a drop operation in a view modified to accept drops.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol DropDelegate
```

## Overview

The DropDelegate protocol provides a comprehensive and flexible way to interact with a drop operation. Specify a drop delegate when you modify a view to accept drops with the onDrop(of:delegate:) method.

Alternatively, for simple drop cases that don’t require the full functionality of a drop delegate, you can modify a view to accept drops using the onDrop(of:isTargeted:perform:) method. This method handles the drop using a closure you provide as part of the modifier.

## Topics

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

func performDrop(info: DropInfo) -> Bool

Tells the delegate it can request the item provider data from the given information.

**Required**

## See Also

### Moving items using item providers

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func onDrop(of:isTargeted:perform:)

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of:delegate:)

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

struct DropProposal

The behavior of a drop.

enum DropOperation

Operation types that determine how a drag and drop session resolves when the user drops a drag item.

struct DropInfo

The current state of a drop.

