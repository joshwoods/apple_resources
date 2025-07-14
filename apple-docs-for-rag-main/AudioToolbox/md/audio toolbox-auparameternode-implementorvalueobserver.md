

- Audio Toolbox
- AUParameterNode
-  implementorValueObserver 

Instance Property

# implementorValueObserver

The callback for parameter value changes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var implementorValueObserver: AUImplementorValueObserver { get set }
```

## Discussion

This block receives all externally-generated changes to parameter values. It should store the new value in its audio signal processing state (assuming that state is separate from the parameter object).

## See Also

### Audio Unit Implementations

var implementorValueProvider: AUImplementorValueProvider

The callback for refreshing known stale values in a parameter tree.

var implementorStringFromValueCallback: AUImplementorStringFromValueCallback

The callback for providing a string representation of a parameter value.

var implementorValueFromStringCallback: AUImplementorValueFromStringCallback

The callback for converting a string to a parameter value.

var implementorDisplayNameWithLengthCallback: AUImplementorDisplayNameWithLengthCallback

The callback for obtaining an abbreviated version of a parameter node display name.

