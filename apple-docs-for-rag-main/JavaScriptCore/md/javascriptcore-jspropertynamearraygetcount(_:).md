

- JavaScriptCore
-  JSPropertyNameArrayGetCount(\_:) 

Function

# JSPropertyNameArrayGetCount(\_:)

Gets a count of the number of items in a JavaScript property name array.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSPropertyNameArrayGetCount(_ array: JSPropertyNameArrayRef!) -> Int
```

## Parameters 

`array`  

The array to retrieve the count from.

## Return Value

An integer count of the number of names in `array`.

## See Also

### Working with Properties

func JSPropertyNameAccumulatorAddName(JSPropertyNameAccumulatorRef!, JSStringRef!)

Adds a property name to a JavaScript property name accumulator.

func JSPropertyNameArrayGetNameAtIndex(JSPropertyNameArrayRef!, Int) -> JSStringRef!

Gets a property name at a specified index in a JavaScript property name array.

func JSPropertyNameArrayRelease(JSPropertyNameArrayRef!)

Releases a JavaScript property name array.

func JSPropertyNameArrayRetain(JSPropertyNameArrayRef!) -> JSPropertyNameArrayRef!

Retains a JavaScript property name array.

typealias JSPropertyAttributes

A set of JavaScript property attributes.

JSPropertyAttribute

A JavaScript property attribute.

typealias JSPropertyNameArrayRef

An array of JavaScript property names.

typealias JSPropertyNameAccumulatorRef

An ordered set of the names of a JavaScript object’s properties.

