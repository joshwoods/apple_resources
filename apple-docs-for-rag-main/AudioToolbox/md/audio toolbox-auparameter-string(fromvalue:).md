

- Audio Toolbox
- AUParameter
-  string(fromValue:) 

Instance Method

# string(fromValue:)

Gets the string representation of a parameter value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func string(fromValue value: UnsafePointer?) -> String
```

## Parameters 

`value`  

The parameter value to represent as a string.

## Return Value

The string representation of a parameter value.

## Discussion

Pass `nil` into the `value` parameter to use the current value.

## See Also

### Managing Parameter Values

var value: AUValue

The parameter’s current value.

func setValue(AUValue, originator: AUParameterObserverToken?)

Sets the parameter’s value, avoiding redundant notifications to the originator.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64)

Sets the parameter’s value, preserving the host time of the gesture that initiated the change.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64, eventType: AUParameterAutomationEventType)

func value(from: String) -> AUValue

Converts a string into a parameter value.

