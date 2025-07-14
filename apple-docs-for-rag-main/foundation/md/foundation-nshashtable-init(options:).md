

- Foundation
- NSHashTable
-  init(options:) 

Initializer

# init(options:)

Returns a hash table with given pointer functions options.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(options: NSPointerFunctions.Options = [])
```

## Parameters 

`options`  

A bit field that specifies the options for the elements in the hash table. For possible values, see NSHashTableOptions.

## Return Value

A hash table with given pointer functions options.

## See Also

### Convenience Constructors

class func weakObjects() -> NSHashTable&lt;ObjectType>

Returns a new hash table for storing weak references to its contents.

