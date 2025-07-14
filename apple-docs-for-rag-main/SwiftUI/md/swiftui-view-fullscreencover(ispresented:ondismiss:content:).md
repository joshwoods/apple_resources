

- SwiftUI
- View
-  fullScreenCover(isPresented:onDismiss:content:) 

Instance Method

# fullScreenCover(isPresented:onDismiss:content:)

Presents a modal view that covers as much of the screen as possible when binding to a Boolean value you provide is true.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func fullScreenCover(
    isPresented: Binding,
    onDismiss: (() -> Void)? = nil,
    @ViewBuilder content: @escaping () -> Content
) -> some View where Content : View
```

## Parameters 

`isPresented`  

A binding to a Boolean value that determines whether to present the sheet.

`onDismiss`  

The closure to execute when dismissing the modal view.

`content`  

A closure that returns the content of the modal view.

## Discussion

Use this method to show a modal view that covers as much of the screen as possible. The example below displays a custom view when the user toggles the value of the `isPresenting` binding:

```
struct FullScreenCoverPresentedOnDismiss: View {
    @State private var isPresenting = false
    var body: some View {
        Button("Present Full-Screen Cover") {
            isPresenting.toggle()
        }
        .fullScreenCover(isPresented: $isPresenting,
                         onDismiss: didDismiss) {
            VStack {
                Text("A full-screen modal view.")
                    .font(.title)
                Text("Tap to Dismiss")
            }
            .onTapGesture {
                isPresenting.toggle()
            }
            .foregroundColor(.white)
            .frame(maxWidth: .infinity,
                   maxHeight: .infinity)
            .background(Color.blue)
            .ignoresSafeArea(edges: .all)
        }
    }

    func didDismiss() {
        // Handle the dismissing action.
    }
}
```

## See Also

### Showing a sheet, cover, or popover

func sheet&lt;Content>(isPresented: Binding&lt;Bool>, onDismiss: (() -> Void)?, content: () -> Content) -> some View

Presents a sheet when a binding to a Boolean value that you provide is true.

func sheet&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a sheet using the given item as a data source for the sheet’s content.

func fullScreenCover&lt;Item, Content>(item: Binding&lt;Item?>, onDismiss: (() -> Void)?, content: (Item) -> Content) -> some View

Presents a modal view that covers as much of the screen as possible using the binding you provide as a data source for the sheet’s content.

func popover&lt;Item, Content>(item: Binding&lt;Item?>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: (Item) -> Content) -> some View

Presents a popover using the given item as a data source for the popover’s content.

func popover&lt;Content>(isPresented: Binding&lt;Bool>, attachmentAnchor: PopoverAttachmentAnchor, arrowEdge: Edge?, content: () -> Content) -> some View

Presents a popover when a given condition is true.

enum PopoverAttachmentAnchor

An attachment anchor for a popover.

