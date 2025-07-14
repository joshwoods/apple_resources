

- SwiftUI
- TabContent
-  popover(isPresented:attachmentAnchor:arrowEdge:content:) 

Instance Method

# popover(isPresented:attachmentAnchor:arrowEdge:content:)

Presents a popover when a given condition is true.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func popover(
    isPresented: Binding,
    attachmentAnchor: PopoverAttachmentAnchor = .rect(.bounds),
    arrowEdge: Edge? = nil,
    @ViewBuilder content: @escaping () -> Content
) -> some TabContent where Content : View
```

## Parameters 

`isPresented`  

A binding to a Boolean value that determines whether to present the popover content that you return from the modifier’s `content` closure.

`attachmentAnchor`  

The positioning anchor that defines the attachment point of the popover. The default is bounds.

`arrowEdge`  

The edge of the `attachmentAnchor` that defines the location of the popover’s arrow in macOS. The default is Edge.top.

`content`  

A closure returning the content of the popover.

## Discussion

Use this method to show a popover whose contents are a SwiftUI view that you provide when a bound Boolean variable is `true`. In the example below, a popover displays whenever the user toggles the `isShowingPopover` state variable by pressing the “Show Popover” button:

```
struct PopoverExample: View {
    @State private var isShowingPopover = false

    var body: some View {
        TabView {
            Tab("Popover Anchor", systemImage: "arrow.down") {
                Button("Show Popover") {
                    self.isShowingPopover = true
                }
            }
            .popover(isPresented: $isShowingPopover) {
                Text("Popover Content")
                    .padding()
            }
        }
    }
}
```

