

- RealityKit
- RealityView
-  blur(radius:opaque:) 

Instance Method

# blur(radius:opaque:)

Applies a Gaussian blur to this view.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func blur(
    radius: CGFloat,
    opaque: Bool = false
) -> some View
```

## Parameters 

`radius`  

The radial size of the blur. A blur is more diffuse when its radius is large.

`opaque`  

A Boolean value that indicates whether the blur renderer permits transparency in the blur output. Set to `true` to create an opaque blur, or set to `false` to permit transparency.

## Discussion

Use `blur(radius:opaque:)` to apply a gaussian blur effect to the rendering of this view.

The example below shows two `Text` views, the first with no blur effects, the second with `blur(radius:opaque:)` applied with the `radius` set to `2`. The larger the radius, the more diffuse the effect.

```
struct Blur: View {
    var body: some View {
        VStack {
            Text("This is some text.")
                .padding()
            Text("This is some blurry text.")
                .blur(radius: 2.0)
        }
    }
}
```

