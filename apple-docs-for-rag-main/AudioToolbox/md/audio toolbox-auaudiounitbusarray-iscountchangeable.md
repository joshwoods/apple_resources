

- Audio Toolbox
- AUAudioUnitBusArray
-  isCountChangeable 

Instance Property

# isCountChangeable

Determines whether the array can have a variable number of busses.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isCountChangeable: Bool { get }
```

## Discussion

The base implementation default value is false.

## See Also

### Bus Array Methods and Properties

var count: Int

The number of busses in the array.

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

func removeObserver(fromAllBusses: NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Removes a KVO observer for a given property on all busses in the array.

