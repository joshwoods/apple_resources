

- Foundation
- NSMapTable
-  init(keyOptions:valueOptions:capacity:) 

Initializer

# init(keyOptions:valueOptions:capacity:)

Returns a map table, initialized with the given options.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    keyOptions: NSPointerFunctions.Options = [],
    valueOptions: NSPointerFunctions.Options = [],
    capacity initialCapacity: Int
)
```

## Parameters 

`keyOptions`  

A bit field that specifies the options for the keys in the map table. For possible values, see NSMapTableOptions.

`valueOptions`  

A bit field that specifies the options for the values in the map table. For possible values, see NSMapTableOptions.

`initialCapacity`  

The initial capacity of the map table. This is just a hint; the map table may subsequently grow and shrink as required.

## Return Value

A map table initialized using the given options.

## Discussion

`values` must contain entries at all the indexes specified in `keys`.

## See Also

### Related Documentation

Collections Programming Topics

### Creating and Initializing a Map Table

init(keyOptions: NSPointerFunctions.Options, valueOptions: NSPointerFunctions.Options)

Returns a new map table, initialized with the given options

init(keyPointerFunctions: NSPointerFunctions, valuePointerFunctions: NSPointerFunctions, capacity: Int)

Returns a map table, initialized with the given functions.

class func strongToStrongObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has strong references to the keys and values.

class func weakToStrongObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has weak references to the keys and strong references to the values.

class func strongToWeakObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has strong references to the keys and weak references to the values.

class func weakToWeakObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has weak references to the keys and values.

typealias NSMapTableOptions

Constants used as components in a bitfield to specify the behavior of elements (keys and values) in an `NSMapTable` object.

