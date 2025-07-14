

- SwiftUI
-  PreviewPlatform 

Enumeration

# PreviewPlatform

Platforms that can run the preview.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum PreviewPlatform
```

## Overview

Xcode infers the platform for a preview based on the currently selected target. If you have a multiplatform target and want to suggest a particular target for a preview, implement the platform computed property as a hint, and specify one of the preview platforms:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
    }

    static var platform: PreviewPlatform? {
        PreviewPlatform.tvOS
    }
}
```

## Topics

### Getting an operating system

case iOS

Specifies iOS as the preview platform.

case macOS

Specifies macOS as the preview platform.

case tvOS

Specifies tvOS as the preview platform.

case watchOS

Specifies watchOS as the preview platform.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Defining a preview

macro Previewable()

Tag allowing a dynamic property to appear inline in a preview.

protocol PreviewProvider

A type that produces view previews in Xcode.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

protocol PreviewModifier

A type that defines an environment in which previews can appear.

struct PreviewModifierContent

The type-erased content of a preview.

