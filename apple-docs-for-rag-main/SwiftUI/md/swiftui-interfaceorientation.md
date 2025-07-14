

- SwiftUI
-  InterfaceOrientation 

Structure

# InterfaceOrientation

The orientation of the interface from the user’s perspective.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct InterfaceOrientation
```

## Overview

By default, device previews appear right side up, using orientation portrait. You can change the orientation with a call to the previewInterfaceOrientation(_:) modifier:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewInterfaceOrientation(.landscapeRight)
    }
}
```

## Topics

### Getting an orientation

static let portrait: InterfaceOrientation

The device is in portrait mode, with the top of the device on top.

static let portraitUpsideDown: InterfaceOrientation

The device is in portrait mode, but is upside down.

static let landscapeLeft: InterfaceOrientation

The device is in landscape mode, with the top of the device on the left.

static let landscapeRight: InterfaceOrientation

The device is in landscape mode, with the top of the device on the right.

## Relationships

### Conforms To

- CaseIterable
- Equatable
- Identifiable
- Sendable

## See Also

### Customizing a preview

func previewDevice(PreviewDevice?) -> some View

Overrides the device for a preview.

struct PreviewDevice

A simulator device that runs a preview.

func previewLayout(PreviewLayout) -> some View

Overrides the size of the container for the preview.

func previewInterfaceOrientation(InterfaceOrientation) -> some View

Overrides the orientation of the preview.

