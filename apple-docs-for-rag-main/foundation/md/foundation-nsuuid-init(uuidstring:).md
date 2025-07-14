

- Foundation
- NSUUID
-  init(uuidString:) 

Initializer

# init(uuidString:)

Initializes a new UUID with the formatted string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(uuidString string: String)
```

## Parameters 

`string`  

The source string containing the UUID. The standard format for UUIDs represented in ASCII is a string punctuated by hyphens, for example `68753A44-4D6F-1226-9C60-0050E4C00067`.

## Return Value

A new UUID object. Returns `nil` for invalid strings.

## See Also

### Creating UUIDs

init()

Initializes a new UUID with RFC 4122 version 4 random bytes.

convenience init(uuidBytes: UnsafePointer&lt;UInt8>?)

Initializes a new UUID with the given bytes.

