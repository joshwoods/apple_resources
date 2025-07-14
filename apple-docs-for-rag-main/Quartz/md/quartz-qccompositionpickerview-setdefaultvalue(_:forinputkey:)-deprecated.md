

- Quartz
- QCCompositionPickerView
-  setDefaultValue(\_:forInputKey:) Deprecated

Instance Method

# setDefaultValue(\_:forInputKey:)

Sets the default value to use for a composition input parameter.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func setDefaultValue(
    _ value: Any!,
    forInputKey key: String!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`value`  

This default value overrides any initial value existing for composition input parameters with this key. Pass `nil` to clear the default value.

`key`  

The input parameter key whose default value you want to set.

## See Also

### Setting Composition Input Parameters

func resetDefaultInputValues()

Clears all previously set default values for composition input parameters.

Deprecated

