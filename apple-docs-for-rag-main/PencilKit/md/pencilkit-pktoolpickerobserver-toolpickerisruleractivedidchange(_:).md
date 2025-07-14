

- PencilKit
- PKToolPickerObserver
-  toolPickerIsRulerActiveDidChange(\_:) 

Instance Method

# toolPickerIsRulerActiveDidChange(\_:)

Tells the observer when a person shows or hides the ruler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func toolPickerIsRulerActiveDidChange(_ toolPicker: PKToolPicker)
```

## Parameters 

`toolPicker`  

The tool picker whose configuration changed.

## See Also

### Detecting tool configuration changes

func toolPickerSelectedToolItemDidChange(PKToolPicker)

Tells the observer when a person selects a new tool item.

