

- Objective-C Runtime
- NSObject
-  compositionParameterView(\_:didChangeParameterWithKey:) Deprecated

Instance Method

# compositionParameterView(\_:didChangeParameterWithKey:)

Called after an input parameter in the composition parameter view has been edited.

macOS 10.4–10.15Deprecated

``` source
func compositionParameterView(
    _ parameterView: QCCompositionParameterView!,
    didChangeParameterWithKey portKey: String!
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`parameterView`  

The composition parameter view in which the parameter changed.

`portKey`  

A key for one of the composition parameters, which is provided to you by the Quartz Composer engine.

