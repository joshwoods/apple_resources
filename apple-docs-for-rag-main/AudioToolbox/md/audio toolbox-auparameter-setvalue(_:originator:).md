

- Audio Toolbox
- AUParameter
-  setValue(\_:originator:) 

Instance Method

# setValue(\_:originator:)

Sets the parameter’s value, avoiding redundant notifications to the originator.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setValue(
    _ value: AUValue,
    originator: AUParameterObserverToken?
)
```

## Parameters 

`value`  

The parameter’s new value.

`originator`  

The originator of the change in value. This token allows for observer management to avoid notification callback loops.

## See Also

### Managing Parameter Values

var value: AUValue

The parameter’s current value.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64)

Sets the parameter’s value, preserving the host time of the gesture that initiated the change.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64, eventType: AUParameterAutomationEventType)

func string(fromValue: UnsafePointer&lt;AUValue>?) -> String

Gets the string representation of a parameter value.

func value(from: String) -> AUValue

Converts a string into a parameter value.

