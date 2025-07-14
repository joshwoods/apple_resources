

- DockKit
- DockAccessory
-  setFramingMode(\_:) 

Instance Method

# setFramingMode(\_:)

Customize the dock accessory’s tracking behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final func setFramingMode(_ mode: DockAccessory.FramingMode) async throws
```

## Parameters 

`mode`  

The framing mode to set tracking to. See DockAccessory.FramingMode for more information.

## Discussion

Use this method to change where DockKit places a subject within the frame. For example, a face may be on the left or right side within the video. If you disable system tracking, this setting applies locally to the current dock accessory only. Otherwise, this setting applies to any active camera stream.

Set the frame mode to the desired value before performing your own custom tracking.

The default is DockAccessory.FramingMode.automatic. See DockAccessory.FramingMode for other values you can use to override.

Throws

DockKitError.notConnected if device isn’t connected, or DockKitError.notSupported in macOS.

## See Also

### Setting framing mode

var framingMode: DockAccessory.FramingMode

The current framing mode.

enum FramingMode

The mode to control framing of the subject when tracking.

