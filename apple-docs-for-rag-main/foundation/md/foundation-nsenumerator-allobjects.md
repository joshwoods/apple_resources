

- Foundation
- NSEnumerator
-  allObjects 

Instance Property

# allObjects

The array of unenumerated objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allObjects: [Any] { get }
```

## Discussion

This array contains all the remaining objects of the enumerator in enumerated order. It does not contain objects that have already been enumerated with previous nextObject() messages.

Accessing this property exhausts the enumerator’s collection so that subsequent invocations of nextObject() return `nil`.

## See Also

### Related Documentation

Collections Programming Topics

### Getting the Enumerated Objects

func nextObject() -> Any?

Returns the next object from the collection being enumerated.

