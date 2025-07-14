

- Objective-C Runtime
- NSObject
-  indicesOfObjects(byEvaluatingObjectSpecifier:) 

Instance Method

# indicesOfObjects(byEvaluatingObjectSpecifier:)

Returns the indices of the specified container objects.

Mac CatalystmacOS

``` source
func indicesOfObjects(byEvaluatingObjectSpecifier specifier: NSScriptObjectSpecifier) -> [NSNumber]?
```

## Parameters 

`specifier`  

An object specifier for the container objects for which to obtain the indices.

## Return Value

A zero-based array of `NSNumber` objects that identify the zero-based indices of the container objects that match `specifier`, or `nil` if no matching objects were found.

## Discussion

Containers that want to evaluate some specifiers on their own should implement this method. If this method returns `nil`, the object specifier will go on to do its own evaluation, so you should only return `nil` if that’s the behavior you want, or if an error occurs. If this method returns an array, the object specifier will use the `NSNumber` objects in it as the indices. So, if you evaluate the specifier and there are no objects that match, you should return an empty array, not `nil`. If you find only one object, you should still return its index in an array. Returning an array with a single index where the index is –1 is interpreted to mean all the objects.

For an example implementation, see “Implementing Object Specifiers” in Object Specifiers in Cocoa Scripting Guide

