

- Foundation
- NSUUID
-  init(uuidBytes:) 

Initializer

# init(uuidBytes:)

Initializes a new UUID with the given bytes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(uuidBytes bytes: UnsafePointer?)
```

## Parameters 

`bytes`  

Raw UUID bytes to use to create the UUID.

## Return Value

A new UUID object.

## See Also

### Creating UUIDs

init()

Initializes a new UUID with RFC 4122 version 4 random bytes.

convenience init?(uuidString: String)

Initializes a new UUID with the formatted string.

