

- Core Media
-  CMSimpleQueueGetTypeID() 

Function

# CMSimpleQueueGetTypeID()

Returns the type identifier of sample buffer objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSimpleQueueGetTypeID() -> CFTypeID
```

## Return Value

`CFTypeID` of `CMSimpleQueue` objects.

## Discussion

You can check if a `CFTypeRef` object is a `CMSimpleQueue` object by comparing `CFGetTypeID(object)` with `CMSimpleQueueGetTypeID()`.

