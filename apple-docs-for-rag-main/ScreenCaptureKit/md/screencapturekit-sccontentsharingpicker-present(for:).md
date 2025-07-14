

- ScreenCaptureKit
- SCContentSharingPicker
-  present(for:) 

Instance Method

# present(for:)

Displays the picker with an already running capture stream.

Mac Catalyst 18.2+macOS 14.0+

``` source
func present(for stream: SCStream)
```

## Parameters 

`stream`  

The capture stream to display in the picker.

## See Also

### Picker display

func present()

Displays the picker with no active selection for capture.

func present(using: SCShareableContentStyle)

Displays the picker for a single type of capture selection.

func present(for: SCStream, using: SCShareableContentStyle)

Displays the picker with an existing capture stream, allowing for a single type of capture selection.

