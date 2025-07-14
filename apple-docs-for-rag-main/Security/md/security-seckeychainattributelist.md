

- Security
-  SecKeychainAttributeList 

Structure

# SecKeychainAttributeList

A list of keychain attributes.

macOS 10.0+

``` source
struct SecKeychainAttributeList
```

## Topics

### Instance Properties

var attr: UnsafeMutablePointer&lt;SecKeychainAttribute>?

A pointer to the first keychain attribute in the array.

var count: UInt32

The number of keychain attributes in the array.

### Initializers

init()

init(count: UInt32, attr: UnsafeMutablePointer&lt;SecKeychainAttribute>?)

## Relationships

### Conforms To

- BitwiseCopyable

