

- PencilKit
- PKToolPickerObserver
-  toolPickerVisibilityDidChange(\_:) 

Instance Method

# toolPickerVisibilityDidChange(\_:)

Tells the observer when a person shows or hides the tool picker.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func toolPickerVisibilityDidChange(_ toolPicker: PKToolPicker)
```

## Parameters 

`toolPicker`  

The tool picker whose configuration changed.

## See Also

### Monitoring visibility changes

func toolPickerFramesObscuredDidChange(PKToolPicker)

Tells the observer when the area that the tool picker obscures changes.

