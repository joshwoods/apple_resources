

- Bundle Resources
- Information Property List
-  GPUEjectPolicy 

Property List Key

# GPUEjectPolicy

The preferred system action when an external GPU is connected from the system.

macOS 10.14+

## Details 

Type  

string

## Possible Values 

`relaunch`  

Set this value to allow macOS to quit and relaunch your app with another GPU. Your app can implement the application(_:willEncodeRestorableState:) method to save any state before it quits, and it can implement the application(_:didDecodeRestorableState:) method to restore any saved state after it relaunches.

`wait`  

Set this value to manually respond to the safe disconnect request. Your app must register and respond to the removalRequested notification posted by Metal. macOS waits for your app to remove all references to the external GPU before notifying the user that it’s safe to disconnect the GPU.

`kill`  

Set this value to allow macOS to force your app to quit.

`ignore`  

Tells the system to ignore the disconnect message. Don’t use this key in new macOS apps.

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

GPUSelectionPolicy

The app’s preference for whether it wants to use external graphics processors.

