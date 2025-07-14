

- Image I/O
-  CGImageDestinationCopyTypeIdentifiers() 

Function

# CGImageDestinationCopyTypeIdentifiers()

Returns an array of the uniform type identifiers that are supported for image destinations.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationCopyTypeIdentifiers() -> CFArray
```

## Return Value

Returns an array of the uniform type identifiers that image destinations support. For a list of system-declared and third-party identifiers, see Uniform Type Identifiers.

## See Also

### Getting the Image Types

func CGImageDestinationGetTypeID() -> CFTypeID

Returns the unique type identifier of an image destination opaque type.

