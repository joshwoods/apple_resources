

- Security
-  SecKeychainAttribute 

Structure

# SecKeychainAttribute

A structure that holds a single keychain attribute.

macOS 10.0+

``` source
struct SecKeychainAttribute
```

## Topics

### Instance Properties

var data: UnsafeMutableRawPointer?

A pointer to the attribute data.

var length: UInt32

The length of the buffer pointed to by data.

var tag: SecKeychainAttrType

A 4-byte attribute tag.

### Initializers

init()

init(tag: SecKeychainAttrType, length: UInt32, data: UnsafeMutableRawPointer?)

## Relationships

### Conforms To

- BitwiseCopyable

