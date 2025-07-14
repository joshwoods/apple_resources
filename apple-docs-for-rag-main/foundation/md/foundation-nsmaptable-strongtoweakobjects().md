

- Foundation
- NSMapTable
-  strongToWeakObjects() 

Type Method

# strongToWeakObjects()

Returns a new map table object which has strong references to the keys and weak references to the values.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func strongToWeakObjects() -> NSMapTable
```

## Return Value

A new map table object which has strong references to the keys and weak references to the values.

## See Also

### Creating and Initializing a Map Table

init(keyOptions: NSPointerFunctions.Options, valueOptions: NSPointerFunctions.Options, capacity: Int)

Returns a map table, initialized with the given options.

init(keyOptions: NSPointerFunctions.Options, valueOptions: NSPointerFunctions.Options)

Returns a new map table, initialized with the given options

init(keyPointerFunctions: NSPointerFunctions, valuePointerFunctions: NSPointerFunctions, capacity: Int)

Returns a map table, initialized with the given functions.

class func strongToStrongObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has strong references to the keys and values.

class func weakToStrongObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has weak references to the keys and strong references to the values.

class func weakToWeakObjects() -> NSMapTable&lt;KeyType, ObjectType>

Returns a new map table object which has weak references to the keys and values.

typealias NSMapTableOptions

Constants used as components in a bitfield to specify the behavior of elements (keys and values) in an `NSMapTable` object.

