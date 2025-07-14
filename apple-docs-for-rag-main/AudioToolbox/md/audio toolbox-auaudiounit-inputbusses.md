

- Audio Toolbox
- AUAudioUnit
-  inputBusses 

Instance Property

# inputBusses

An array containing the audio unit’s input connection points.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var inputBusses: AUAudioUnitBusArray { get }
```

## Discussion

Subclasses must override this property’s getter. The audio unit should return the same object every time it is asked for it, since hosts can install KVO observers on it.

## See Also

### Returning the Audio Busses

var outputBusses: AUAudioUnitBusArray

An array containing the audio unit’s output connection points.

