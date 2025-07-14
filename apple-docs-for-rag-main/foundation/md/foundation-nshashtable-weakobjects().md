

- Foundation
- NSHashTable
-  weakObjects() 

Type Method

# weakObjects()

Returns a new hash table for storing weak references to its contents.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func weakObjects() -> NSHashTable
```

## Return Value

A new hash table that uses the weakMemory options and objectPersonality and has an initial capacity of `0`.

## See Also

### Convenience Constructors

init(options: NSPointerFunctions.Options)

Returns a hash table with given pointer functions options.

