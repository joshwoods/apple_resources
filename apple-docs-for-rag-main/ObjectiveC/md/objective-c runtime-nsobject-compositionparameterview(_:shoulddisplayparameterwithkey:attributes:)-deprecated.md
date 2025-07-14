

- Objective-C Runtime
- NSObject
-  compositionParameterView(\_:shouldDisplayParameterWithKey:attributes:) Deprecated

Instance Method

# compositionParameterView(\_:shouldDisplayParameterWithKey:attributes:)

Allows you to define which composition parameters are visible in the user interface when the composition parameter view refreshes.

macOS 10.4–10.15Deprecated

``` source
func compositionParameterView(
    _ parameterView: QCCompositionParameterView!,
    shouldDisplayParameterWithKey portKey: String!,
    attributes portAttributes: [AnyHashable : Any]! = [:]
) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`parameterView`  

The composition parameter view in which the selection changed.

`portKey`  

A key for one of the composition parameters, which is provided to you by the Quartz Composer engine.

`portAttributes`  

A dictionary of the attributes that you want to display in the user interface.

## Return Value

ReturnYES if the port attributes should be displayed; NO otherwise.

