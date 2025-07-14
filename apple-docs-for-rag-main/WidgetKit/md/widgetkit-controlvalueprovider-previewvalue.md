

- WidgetKit
- ControlValueProvider
-  previewValue 

Instance Property

# previewValue

A value to be shown while previewing the control in the add sheet.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
var previewValue: Self.Value { get }
```

**Required**

## Discussion

This value should be generated quickly and cheaply. Calculate more expensive and accurate values in currentValue().

