

- SwiftUI
-  ImmersionStyle 

Protocol

# ImmersionStyle

The styles that an immersive space can have.

visionOS 1.0+

``` source
protocol ImmersionStyle
```

## Overview

Configure the appearance and behavior of an ImmersiveSpace by adding the immersionStyle(selection:in:) scene modifier to the space and specifying a style that conforms to this protocol, like mixed or full. For example, the following app defines a solar system scene that uses full immersion:

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

## Topics

### Getting built-in styles

static var automatic: AutomaticImmersionStyle

The default immersion style.

static var full: FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

static var mixed: MixedImmersionStyle

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

static var progressive: ProgressiveImmersionStyle

An immersion style that displays unbounded content that partially replaces passthrough video.

### Supporting types

struct AutomaticImmersionStyle

The default style of immersive spaces.

struct FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

struct MixedImmersionStyle

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

struct ProgressiveImmersionStyle

An immersion style that displays unbounded content that partially replaces passthrough video.

### Type Methods

static progressive(_:initialAmount:)

An immersion style that displays unbounded content that partially replaces passthrough video.

## Relationships

### Conforming Types

- AutomaticImmersionStyle
- FullImmersionStyle
- MixedImmersionStyle
- ProgressiveImmersionStyle

## See Also

### Creating an immersive space

struct ImmersiveSpace

A scene that presents its content in an unbounded space.

struct ImmersiveSpaceContentBuilder

A result builder for composing a collection of immersive space elements.

func immersionStyle(selection: Binding&lt;any ImmersionStyle>, in: any ImmersionStyle...) -> some Scene

Sets the style for an immersive space.

var immersiveSpaceDisplacement: Pose3D

The displacement that the system applies to the immersive space when moving the space away from its default position, in meters.

