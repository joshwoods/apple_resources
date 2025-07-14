

- DeveloperToolsSupport
- PreviewCamera
-  init(lookingAt:from:name:) 

Initializer

# init(lookingAt:from:name:)

Creates a camera that looks towards a specified point in the preview from a different specified point.

visionOS 1.0+

``` source
init(
    lookingAt position: Point3D,
    from: Point3D,
    name: String? = nil
)
```

## Parameters 

`position`  

The point to aim the camera at, specified in meters from the preview center.

`from`  

The position of the camera, specified in meters from the preview center.

`name`  

An optional name that the canvas uses to label the camera.

## Discussion

Use one or more cameras with one of the preview macros that takes a `cameras` input — like Preview(_:traits:body:cameras:) — to create custom viewpoints for the preview. The canvas offers custom cameras in its camera picker along with a set of standard cameras.

