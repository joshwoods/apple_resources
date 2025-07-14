

- Audio Toolbox
- AUAudioUnit
-  parametersForOverview(withCount:) 

Instance Method

# parametersForOverview(withCount:)

Returns the audio unit’s most important parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func parametersForOverview(withCount count: Int) -> [NSNumber]
```

## Parameters 

`count`  

The number of parameters to return.

## Return Value

An array of addresses representing the audio unit’s most important parameters.

## Discussion

This method allows a host to query an audio unit for a small number of its most important parameters, to be displayed in a compact generic view.

This version 3 method is partially bridged to the version 2 `kAudioUnitProperty_ParametersForOverview` API.

## See Also

### Querying Parameters

var parameterTree: AUParameterTree?

An audio unit’s parameters, organized in a tree hierarchy.

var allParameterValues: Bool

Special read-only property for KVO.

