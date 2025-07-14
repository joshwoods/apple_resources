

- MetalKit
- MTKView
-  init(coder:) 

Initializer

# init(coder:)

Initializes a view from data in a given unarchiver.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(coder: NSCoder)
```

## Parameters 

`coder`  

An unarchiver object.

## Return Value

An initialized view object.

## See Also

### Creating a View

init(frame: CGRect, device: (any MTLDevice)?)

Initializes a view with the specified frame rectangle and Metal device.

