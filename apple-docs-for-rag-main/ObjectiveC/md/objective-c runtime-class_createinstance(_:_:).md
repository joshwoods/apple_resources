

- Objective-C Runtime
-  class_createInstance(\_:\_:) 

Function

# class_createInstance(\_:\_:)

Creates an instance of a class, allocating memory for the class in the default malloc memory zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func class_createInstance(
    _ cls: AnyClass?,
    _ extraBytes: Int
) -> Any?
```

## Parameters 

`cls`  

The class that you want to allocate an instance of.

`extraBytes`  

An integer indicating the number of extra bytes to allocate. The additional bytes can be used to store additional instance variables beyond those defined in the class definition.

## Return Value

An instance of the class `cls`.

