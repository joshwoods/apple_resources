

- SwiftUI
-  PreviewProvider 

Protocol

# PreviewProvider

A type that produces view previews in Xcode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
protocol PreviewProvider : _PreviewProvider
```

## Overview

Important

You can use this protocol to define a preview manually, but you typically use a preview macro like Preview(_:body:) instead.

You can create an Xcode preview by declaring a structure that conforms to the `PreviewProvider` protocol. Implement the required previews computed property, and return the view to display:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
    }
}
```

Xcode statically discovers preview providers in your project and generates previews for any providers currently open in the source editor. Xcode generates the preview using the current run destination as a hint for which device to display. For example, Xcode shows the following preview if you’ve selected an iOS target to run on the iPhone 12 Pro Max simulator:

When you create a new file (File \> New \> File) and choose the SwiftUI view template, Xcode automatically inserts a preview structure at the bottom of the file that you can configure. You can also create new preview structures in an existing SwiftUI view file by choosing Editor \> Create Preview.

Customize the preview’s appearance by adding view modifiers, just like you do when building a custom View. This includes preview-specific modifiers that let you control aspects of the preview, like the device orientation:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
            .previewInterfaceOrientation(.landscapeLeft)
    }
}
```

For the complete list of preview customizations, see Previews in Xcode.

Xcode creates different previews for each view in your preview, so you can see variations side by side. For example, you might want to see a view’s light and dark appearances simultaneously:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        CircleImage()
        CircleImage()
            .preferredColorScheme(.dark)
    }
}
```

Use a Group when you want to maintain different previews, but apply a single modifier to all of them:

```
struct CircleImage_Previews: PreviewProvider {
    static var previews: some View {
        Group {
            CircleImage()
            CircleImage()
                .preferredColorScheme(.dark)
        }
        .previewLayout(.sizeThatFits)
    }
}
```

## Topics

### Creating a preview

static var previews: Self.Previews

A collection of views to preview.

**Required**

associatedtype Previews : View

The type to preview.

**Required**

### Specifying the platform

static var platform: PreviewPlatform?

The platform on which to run the provider.

**Required** Default implementation provided.

## See Also

### Defining a preview

macro Previewable()

Tag allowing a dynamic property to appear inline in a preview.

enum PreviewPlatform

Platforms that can run the preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

protocol PreviewModifier

A type that defines an environment in which previews can appear.

struct PreviewModifierContent

The type-erased content of a preview.

