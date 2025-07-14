

- WidgetKit
- AppIntentControlValueProvider
-  previewValue(configuration:) 

Instance Method

# previewValue(configuration:)

A value to be shown while previewing the control in the add sheet.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func previewValue(configuration: Self.Configuration) -> Self.Value
```

**Required**

## Parameters 

`configuration`  

The intent containing user-editable parameters.

## Discussion

This value should be generated quickly and cheaply. Calculate more expensive and accurate values in currentValue(configuration:).

