

- Foundation
- NSDictionary
-  init(object:forKey:) 

Initializer

# init(object:forKey:)

Creates a dictionary containing a given key and value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    object: Any,
    forKey key: any NSCopying
)
```

## Parameters 

`object`  

The value corresponding to `aKey`.

If this value is `nil`, an invalidArgumentException is raised.

`key`  

The key for `anObject`.

If this value is `nil`, an invalidArgumentException is raised.

## Return Value

A new dictionary containing a single object, `object`, for a single key, `aKey`.

## See Also

### Creating a Dictionary from Objects and Keys

convenience init(objects: [Any], forKeys: [any NSCopying])

Initializes a newly allocated dictionary with key-value pairs constructed from the provided arrays of keys and objects.

init(objects: UnsafePointer&lt;AnyObject>?, forKeys: UnsafePointer&lt;any NSCopying>?, count: Int)

Initializes a newly allocated dictionary with the specified number of key-value pairs constructed from the provided C arrays of keys and objects.

