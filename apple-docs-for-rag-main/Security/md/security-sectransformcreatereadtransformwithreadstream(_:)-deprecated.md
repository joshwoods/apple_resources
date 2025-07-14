

- Security
-  SecTransformCreateReadTransformWithReadStream(\_:) Deprecated

Function

# SecTransformCreateReadTransformWithReadStream(\_:)

Creates a read transform from a read stream reference.

macOS 10.7–13.0Deprecated

``` source
func SecTransformCreateReadTransformWithReadStream(_ inputStream: CFReadStream) -> SecTransform
```

Deprecated

SecTransform is no longer supported

## Parameters 

`inputStream`  

The stream that is to be opened and read from when the chain executes.

## Return Value

A pointer to a new transform. In Objective-C, call the CFRelease function to free this object’s memory when you are done with it.

