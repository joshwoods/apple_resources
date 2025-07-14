

- DeveloperToolsSupport
-  PreviewLayout 

Enumeration

# PreviewLayout

A size constraint for a preview.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum PreviewLayout
```

## Overview

Customize the layout of a preview that you define using the PreviewProvider protocol by providing one of the preview layout values to the previewLayout(_:) view modifier. For example, you can tell the preview to take up only the amount of space that the view requires with PreviewLayout.sizeThatFits:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewLayout(.sizeThatFits)
    }
}
```

Note

When you migrate away from preview providers and to preview macros, you specify layout using one of the PreviewTrait layout values with a macro that takes traits, like Preview(_:traits:_:body:).

## Topics

### Enumeration Cases

case device

Center the preview in a container the size of the device on which the preview is running.

case fixed(width: CGFloat, height: CGFloat)

Center the preview in a fixed size container with the given dimensions.

case fixed3D(width: CGFloat, height: CGFloat, depth: CGFloat)

Centers the preview in a fixed-size, 3D container.

case sizeThatFits

Fit the container to the size of the preview when offered the size of the device that the preview is running on.

## Relationships

### Conforms To

- Sendable

## See Also

### Preview Registration

protocol PreviewRegistry

A protocol that the system uses to locate previews at runtime.

struct Preview

A base type that preview macros use to create previews.

struct PreviewTrait

Customizations that you can apply to a preview.

