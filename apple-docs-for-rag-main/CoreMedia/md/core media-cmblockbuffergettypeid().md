

- Core Media
-  CMBlockBufferGetTypeID() 

Function

# CMBlockBufferGetTypeID()

Returns the type identifier for block buffer objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBlockBufferGetTypeID() -> CFTypeID
```

## Return Value

Returns the `CFTypeID` corresponding to `CMBlockBuffer`.

## Discussion

Obtains the CoreFoundation type ID for the `CMBlockBuffer` type.

