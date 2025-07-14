

- Audio Toolbox
- AUAudioUnit
-  allParameterValues 

Instance Property

# allParameterValues

Special read-only property for KVO.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var allParameterValues: Bool { get }
```

## Discussion

KVO notifications are issued on this property in response to certain events where potentially all parameter values are invalidated—for example, the selection of a preset.

## See Also

### Related Documentation

var fullState: [String : Any]?

A persistable snapshot of the audio unit’s properties and parameters, suitable for saving as a user preset.

### Querying Parameters

var parameterTree: AUParameterTree?

An audio unit’s parameters, organized in a tree hierarchy.

func parametersForOverview(withCount: Int) -> [NSNumber]

Returns the audio unit’s most important parameters.

