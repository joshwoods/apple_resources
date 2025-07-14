

- SwiftUI
-  Previewable() 

Macro

# Previewable()

Tag allowing a dynamic property to appear inline in a preview.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(peer)
macro Previewable()
```

## Overview

Tagging a variable declaration at root scope in your `#Preview` body with ‘@Previewable’ allows you to use dynamic properties inline in previews. The `#Preview` macro will generate an embedded SwiftUI view; tagged declarations become properties on the view, and all remaining statements form the view’s body.

```
#Preview("toggle") {
    @Previewable @State var toggled = true
    return Toggle("Loud Noises", isOn: $toggled)
}
```

It is an error to use `@Previewable` outside of a `#Preview` body closure.

## See Also

### Defining a preview

protocol PreviewProvider

A type that produces view previews in Xcode.

enum PreviewPlatform

Platforms that can run the preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

protocol PreviewModifier

A type that defines an environment in which previews can appear.

struct PreviewModifierContent

The type-erased content of a preview.

