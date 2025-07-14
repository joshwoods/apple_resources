

- MetalKit
- MTKView
-  init(frame:device:) 

Initializer

# init(frame:device:)

Initializes a view with the specified frame rectangle and Metal device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(
    frame frameRect: CGRect,
    device: (any MTLDevice)?
)
```

## Parameters 

`frameRect`  

The frame rectangle for the view.

`device`  

The Metal device object to use.

## Return Value

An initialized view object.

## See Also

### Creating a View

init(coder: NSCoder)

Initializes a view from data in a given unarchiver.

