

- Audio Toolbox
- AUAudioUnitBusArray
-  removeObserver(fromAllBusses:forKeyPath:context:) 

Instance Method

# removeObserver(fromAllBusses:forKeyPath:context:)

Removes a KVO observer for a given property on all busses in the array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeObserver(
    fromAllBusses observer: NSObject,
    forKeyPath keyPath: String,
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`observer`  

The KVO observer.

`keyPath`  

The property’s key path.

`context`  

The KVO context.

## See Also

### Bus Array Methods and Properties

var count: Int

The number of busses in the array.

var isCountChangeable: Bool

Determines whether the array can have a variable number of busses.

var ownerAudioUnit: AUAudioUnit

The audio unit that owns the bus array.

var busType: AUAudioUnitBusType

Determines whether the bus array is for input or output.

subscript(Int) -> AUAudioUnitBus

Returns the bus at the specified index.

func setBusCount(Int) throws

Changes the number of busses in the array.

func addObserver(toAllBusses: NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Adds a KVO observer for a given property on all busses in the array.

