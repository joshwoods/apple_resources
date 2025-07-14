

- Bundle Resources
- Information Property List
-  GPUSelectionPolicy 

Property List Key

# GPUSelectionPolicy

The app’s preference for whether it wants to use external graphics processors.

macOS 10.14+

## Details 

Type  

string

## Possible Values 

`avoidRemovable`  

Metal tries to avoid creating contexts on external GPUs. For legacy OpenGL apps, OpenGL also avoids creating contexts using external GPUs. Set this option only if your app doesn’t support external GPU event handling.

`preferRemovable`  

If external GPUs are visible to the system, Metal prefers them over other GPUs. Similarly, for legacy OpenGL apps, OpenGL also prefers to create contexts on the external GPU.

## Discussion

This key is optional.

## See Also

### Graphics

UIAppSupportsHDR

A Boolean value that indicates whether the app supports HDR mode on Apple TV 4K.

**Name:** Supports HDR color mode

NSHighResolutionCapable

A Boolean value indicating whether the Cocoa app supports high-resolution displays.

**Name:** High Resolution Capable

NSSupportsAutomaticGraphicsSwitching

A Boolean value indicating whether an OpenGL app may utilize the integrated GPU.

**Name:** Supports Automatic Graphics Switching

GPUEjectPolicy

The preferred system action when an external GPU is connected from the system.

