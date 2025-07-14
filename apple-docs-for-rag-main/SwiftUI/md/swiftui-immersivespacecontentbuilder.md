

- SwiftUI
-  ImmersiveSpaceContentBuilder 

Structure

# ImmersiveSpaceContentBuilder

A result builder for composing a collection of immersive space elements.

visionOS 1.0+

``` source
@resultBuilder
struct ImmersiveSpaceContentBuilder
```

## Topics

### Building content

static func buildBlock&lt;Content>(Content) -> Content

## See Also

### Creating an immersive space

struct ImmersiveSpace

A scene that presents its content in an unbounded space.

func immersionStyle(selection: Binding&lt;any ImmersionStyle>, in: any ImmersionStyle...) -> some Scene

Sets the style for an immersive space.

protocol ImmersionStyle

The styles that an immersive space can have.

var immersiveSpaceDisplacement: Pose3D

The displacement that the system applies to the immersive space when moving the space away from its default position, in meters.

