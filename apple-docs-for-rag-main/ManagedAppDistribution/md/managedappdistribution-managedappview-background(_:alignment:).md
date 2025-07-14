

- ManagedAppDistribution
- ManagedAppView
-  background(\_:alignment:) 

Instance Method

# background(\_:alignment:)

Layers the given view behind this view.

ManagedAppDistributionSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func background(
    _ background: Background,
    alignment: Alignment = .center
) -> some View where Background : View
```

## Parameters 

`background`  

The view to draw behind this view.

`alignment`  

The alignment with a default value of `Alignment/center` that you use to position the background view.

## Discussion

Use `background(_:alignment:)` when you need to place one view behind another, with the background view optionally aligned with a specified edge of the frontmost view.

The example below creates two views: the `Frontmost` view, and the `DiamondBackground` view. The `Frontmost` view uses the `DiamondBackground` view for the background of the image element inside the `Frontmost` view’s `VStack`.

```
struct DiamondBackground: View {
    var body: some View {
        VStack {
            Rectangle()
                .fill(.gray)
                .frame(width: 250, height: 250, alignment: .center)
                .rotationEffect(.degrees(45.0))
        }
    }
}

struct Frontmost: View {
    var body: some View {
        VStack {
            Image(systemName: "folder")
                .font(.system(size: 128, weight: .ultraLight))
                .background(DiamondBackground())
        }
    }
}
```

