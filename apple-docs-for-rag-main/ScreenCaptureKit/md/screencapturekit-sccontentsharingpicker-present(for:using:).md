

- ScreenCaptureKit
- SCContentSharingPicker
-  present(for:using:) 

Instance Method

# present(for:using:)

Displays the picker with an existing capture stream, allowing for a single type of capture selection.

Mac Catalyst 18.2+macOS 14.0+

``` source
func present(
    for stream: SCStream,
    using contentStyle: SCShareableContentStyle
)
```

## Parameters 

`stream`  

The stream to display in the picker.

`contentStyle`  

The type of streaming content selection allowed through the presented picker.

## See Also

### Picker display

func present()

Displays the picker with no active selection for capture.

func present(for: SCStream)

Displays the picker with an already running capture stream.

func present(using: SCShareableContentStyle)

Displays the picker for a single type of capture selection.

