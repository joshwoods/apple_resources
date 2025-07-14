

- DeveloperToolsSupport
-  PreviewTrait 

Structure

# PreviewTrait

Customizations that you can apply to a preview.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor
struct PreviewTrait
```

## Topics

### Initializers

init(PreviewTrait&lt;T>...)

Convenience to compose multiple traits into a single trait.

### Type Properties

static var defaultLayout: PreviewTrait&lt;Preview.ViewTraits>

Center the preview in a container the size of the device on which the preview is running.

static var landscapeLeft: PreviewTrait&lt;Preview.ViewTraits>

The device is in landscape mode, with the top of the device on the left.

static var landscapeRight: PreviewTrait&lt;Preview.ViewTraits>

The device is in landscape mode, with the top of the device on the right.

static var portrait: PreviewTrait&lt;Preview.ViewTraits>

The device is in portrait mode, with the top of the device on top.

static var portraitUpsideDown: PreviewTrait&lt;Preview.ViewTraits>

The device is in portrait mode, but is upside down.

static var sizeThatFitsLayout: PreviewTrait&lt;Preview.ViewTraits>

Fit the container to the size of the preview when offered the size of the device that the preview is running on.

### Type Methods

static func fixedLayout(width: CGFloat, height: CGFloat) -> PreviewTrait&lt;T>

Center the preview in a fixed size container with the given dimensions.

static func fixedLayout(width: CGFloat, height: CGFloat, depth: CGFloat) -> PreviewTrait&lt;T>

Centers the preview in a fixed-size, 3D container.

static func modifier(some PreviewModifier) -> PreviewTrait&lt;T>

Attach a `PreviewModifier` to the preview.

## Relationships

### Conforms To

- Sendable

## See Also

### Preview Registration

protocol PreviewRegistry

A protocol that the system uses to locate previews at runtime.

struct Preview

A base type that preview macros use to create previews.

enum PreviewLayout

A size constraint for a preview.

