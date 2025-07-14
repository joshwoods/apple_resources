

- Core Motion
- CMAttitude
-  multiply(byInverseOf:) 

Instance Method

# multiply(byInverseOf:)

Yields the change in attitude given a specific attitude.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
func multiply(byInverseOf attitude: CMAttitude)
```

## Parameters 

`attitude`  

An object representing the device’s attitude at a given moment of measurement.

## Discussion

This method multiplies the inverse of the specified `CMAttitude` object by the attitude represented by the receiving object. It replaces the receiving instance with the attitude *change* relative to the object passed in `attitude`. You should cache the `CMAttitude` instance you want to use as a reference and pass that object as the argument to subsequent calls of this method.

