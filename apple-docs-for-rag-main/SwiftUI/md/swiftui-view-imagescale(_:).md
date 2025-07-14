

- SwiftUI
- View
-  imageScale(\_:) 

Instance Method

# imageScale(\_:)

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func imageScale(_ scale: Image.Scale) -> some View
```

## Parameters 

`scale`  

One of the relative sizes provided by the image scale enumeration.

## Discussion

The example below shows the relative scaling effect. The system renders the image at a relative size based on the available space and configuration options of the image it is scaling.

```
VStack {
    HStack {
        Image(systemName: "heart.fill")
            .imageScale(.small)
        Text("Small")
    }
    HStack {
        Image(systemName: "heart.fill")
            .imageScale(.medium)
        Text("Medium")
    }

    HStack {
        Image(systemName: "heart.fill")
            .imageScale(.large)
        Text("Large")
    }
}
```

## See Also

### Configuring an image

Fitting images into available space

Adjust the size and shape of images in your app’s user interface by applying view modifiers.

var imageScale: Image.Scale

The image scale for this environment.

enum Scale

A scale to apply to vector images relative to text.

enum Orientation

The orientation of an image.

enum ResizingMode

The modes that SwiftUI uses to resize an image to fit within its containing view.

