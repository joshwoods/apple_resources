

- Media Accessibility
- MAFlashingLightsProcessor
-  canProcessSurface(\_:) 

Instance Method

# canProcessSurface(\_:)

Returns a Boolean value that indicates whether the flashing lights processor can process the content in the surface for sequences of flashing lights.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func canProcessSurface(_ surface: IOSurfaceRef) -> Bool
```

## Parameters 

`surface`  

The IOSurfaceRef to process for flashing lights.

## Return Value

true if the processor can process the content in the surface for flashing lights. false if the processor can’t process the surface, which can occur for unsupported hardware or unsupported color spaces.

