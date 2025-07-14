

- SwiftUI
- Scene
-  immersionStyle(selection:in:) 

Instance Method

# immersionStyle(selection:in:)

Sets the style for an immersive space.

visionOS 1.0+

``` source
nonisolated
func immersionStyle(
    selection: Binding,
    in styles: any ImmersionStyle...
) -> some Scene
```

## Parameters 

`selection`  

A Binding to the style that the space uses. You can change this value to change the scene’s style even after you present the immersive space. Even though you provide a binding, the value changes only if you change it.

`styles`  

The list of styles that the `selection` input can have. Include any styles that you plan to use during the lifetime of the scene.

## Return Value

A scene that uses one of the specified `styles`.

## Discussion

Use this modifier to configure the appearance and behavior of an ImmersiveSpace. Specify a style that conforms to the ImmersionStyle protocol, like mixed or full. For example, the following app defines a solar system scene that uses full immersion:

```
@main
struct SolarSystemApp: App {
    @State private var style: ImmersionStyle = .full

    var body: some Scene {
        ImmersiveSpace {
            SolarSystem()
        }
        .immersionStyle(selection: $style, in: .full)
    }
}
```

## See Also

### Creating an immersive space

struct ImmersiveSpace

A scene that presents its content in an unbounded space.

struct ImmersiveSpaceContentBuilder

A result builder for composing a collection of immersive space elements.

protocol ImmersionStyle

The styles that an immersive space can have.

var immersiveSpaceDisplacement: Pose3D

The displacement that the system applies to the immersive space when moving the space away from its default position, in meters.

