

- ScreenCaptureKit
- SCContentSharingPicker
-  present(using:) 

Instance Method

# present(using:)

Displays the picker for a single type of capture selection.

Mac Catalyst 18.2+macOS 14.0+

``` source
func present(using contentStyle: SCShareableContentStyle)
```

## Parameters 

`contentStyle`  

The type of streaming content selection allowed through the presented picker.

## See Also

### Picker display

func present()

Displays the picker with no active selection for capture.

func present(for: SCStream)

Displays the picker with an already running capture stream.

func present(for: SCStream, using: SCShareableContentStyle)

Displays the picker with an existing capture stream, allowing for a single type of capture selection.

