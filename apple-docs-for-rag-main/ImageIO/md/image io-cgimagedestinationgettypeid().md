

- Image I/O
-  CGImageDestinationGetTypeID() 

Function

# CGImageDestinationGetTypeID()

Returns the unique type identifier of an image destination opaque type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationGetTypeID() -> CFTypeID
```

## Return Value

Returns the Core Foundation type ID for an image destination.

## Discussion

A type identifier is an integer that identifies the opaque type to which a Core Foundation object belongs. You use type IDs in various contexts, such as when you are operating on heterogeneous collections.

## See Also

### Getting the Image Types

func CGImageDestinationCopyTypeIdentifiers() -> CFArray

Returns an array of the uniform type identifiers that are supported for image destinations.

