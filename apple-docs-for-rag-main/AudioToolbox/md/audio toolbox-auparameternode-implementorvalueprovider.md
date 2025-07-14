

- Audio Toolbox
- AUParameterNode
-  implementorValueProvider 

Instance Property

# implementorValueProvider

The callback for refreshing known stale values in a parameter tree.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var implementorValueProvider: AUImplementorValueProvider { get set }
```

## Discussion

The audio unit should return the current value for this parameter; the parameter node object then stores this value.

## See Also

### Audio Unit Implementations

var implementorValueObserver: AUImplementorValueObserver

The callback for parameter value changes.

var implementorStringFromValueCallback: AUImplementorStringFromValueCallback

The callback for providing a string representation of a parameter value.

var implementorValueFromStringCallback: AUImplementorValueFromStringCallback

The callback for converting a string to a parameter value.

var implementorDisplayNameWithLengthCallback: AUImplementorDisplayNameWithLengthCallback

The callback for obtaining an abbreviated version of a parameter node display name.

