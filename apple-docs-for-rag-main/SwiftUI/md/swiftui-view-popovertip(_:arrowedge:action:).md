

- SwiftUI
- View
-  popoverTip(\_:arrowEdge:action:) 

Instance Method

# popoverTip(\_:arrowEdge:action:)

Presents a popover tip on the modified view.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+

``` source
@MainActor @preconcurrency
func popoverTip(
    _ tip: (any Tip)?,
    arrowEdge: Edge? = nil,
    action: @escaping (Tips.Action) -> Void = { _ in }
) -> some View
```

## Parameters 

`tip`  

The tip to display.

`arrowEdge`  

The edge of the attachmentAnchor that defines the location of the popover’s arrow. By default, the system will choose the best orientation of the popover’s arrow.

`action`  

The action to perform when the user triggers a tip’s button.

### Discussion

Use this modifier to present a tip as a popover on an existing view when the tip becomes eligible for display.

```
import SwiftUI
import TipKit

// Define your tip's content.
struct SampleTip: Tip {
    var title: Text {
        Text("Save as a Favorite")
    }

    var message: Text? {
        Text("Your favorite backyards always appear at the top of the list.")
    }

    var image: Image? {
        Image(systemName: "star")
    }
}

struct SampleView: View {
    // Create an instance of your tip.
    var tip = SampleTip()

    var body: some View {
        VStack {
            // Add `.popoverTip` to the view you want to modify.
            // Tips.configure(options:) must be called before your tip will be eligible for display.
            Image(systemName: "star")
                .popoverTip(tip)
        }
    }
}
```

## See Also

### Providing tips

func tipBackground(some ShapeStyle) -> some View

Sets the tip’s view background to a style. Currently this only applies to inline tips, not popover tips.

func tipCornerRadius(CGFloat, antialiased: Bool) -> some View

Sets the corner radius for an inline tip view.

func tipImageSize(CGSize) -> some View

Sets the size for a tip’s image.

func tipViewStyle(some TipViewStyle) -> some View

Sets the given style for TipView within the view hierarchy.

func tipImageStyle&lt;S>(S) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2>(S1, S2) -> some View

Sets the style for a tip’s image.

func tipImageStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the style for a tip’s image.

