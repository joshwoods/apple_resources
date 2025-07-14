

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  imageScale(\_:) 

Instance Method

# imageScale(\_:)

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 11.0+tvOS 13.0+watchOS 6.0+

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

