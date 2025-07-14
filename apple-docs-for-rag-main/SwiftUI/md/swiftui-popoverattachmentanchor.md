

- SwiftUI
-  PopoverAttachmentAnchor 

Enumeration

# PopoverAttachmentAnchor

An attachment anchor for a popover.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum PopoverAttachmentAnchor
```

## Topics

### Getting attachment anchors

case point(UnitPoint)

The anchor point for the popover expressed as a unit point that describes possible alignments relative to a SwiftUI view.

case rect(Anchor&lt;CGRect>.Source)

The anchor point for the popover relative to the source’s frame.

## See Also

### Showing a sheet, cover, or popover

func sheet&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a sheet when a binding to a Boolean value that you provide is true.

func sheet&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a sheet using the given item as a data source for the sheet’s content.

func fullScreenCover&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a modal view that covers as much of the screen as possible when binding to a Boolean value you provide is true.

func fullScreenCover&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a modal view that covers as much of the screen as possible using the binding you provide as a data source for the sheet’s content.

func popover&lt;Item, Content>(item: Binding&lt;Item?>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: (Item) -> Content) -> some View

Presents a popover using the given item as a data source for the popover’s content.

func popover&lt;Content>(isPresented: Binding&lt;Bool>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: () -> Content) -> some View

Presents a popover when a given condition is true.

