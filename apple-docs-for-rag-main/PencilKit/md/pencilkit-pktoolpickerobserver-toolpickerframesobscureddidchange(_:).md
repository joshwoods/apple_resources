

- PencilKit
- PKToolPickerObserver
-  toolPickerFramesObscuredDidChange(\_:) 

Instance Method

# toolPickerFramesObscuredDidChange(\_:)

Tells the observer when the area that the tool picker obscures changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func toolPickerFramesObscuredDidChange(_ toolPicker: PKToolPicker)
```

## Parameters 

`toolPicker`  

The tool picker whose configuration changed.

## See Also

### Monitoring visibility changes

func toolPickerVisibilityDidChange(PKToolPicker)

Tells the observer when a person shows or hides the tool picker.

