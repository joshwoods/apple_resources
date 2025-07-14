

- Audio Toolbox
- AUAudioUnitBusArray
-  setBusCount(\_:) 

Instance Method

# setBusCount(\_:)

Changes the number of busses in the array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setBusCount(_ count: Int) throws
```

## Parameters 

`count`  

The new number of busses in the array.

## Discussion

- false if the operation failed.

## Discussion

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

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

func addObserver(toAllBusses: NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Adds a KVO observer for a given property on all busses in the array.

func removeObserver(fromAllBusses: NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Removes a KVO observer for a given property on all busses in the array.

