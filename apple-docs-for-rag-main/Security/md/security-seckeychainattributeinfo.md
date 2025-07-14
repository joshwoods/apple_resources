

- Security
-  SecKeychainAttributeInfo 

Structure

# SecKeychainAttributeInfo

A structure that represents an attribute.

macOS 10.0+

``` source
struct SecKeychainAttributeInfo
```

## Overview

Each tag and format item form a pair. Use SecKeychainAttributeInfoForItemID(_:_:_:) to obtain the structure for a given keychain item, and SecKeychainFreeAttributeInfo(_:) to release that structure’s memory when you are done with it. Use an instance of this structure in a call to the SecKeychainItemCopyAttributesAndData(_:_:_:_:_:_:) function to specify the attributes of a keychain item to retrieve.

## Topics

### Instance Properties

var count: UInt32

The number of tag-format pairs in the respective arrays.

var format: UnsafeMutablePointer&lt;UInt32>?

A pointer to the first attribute format in the array.

var tag: UnsafeMutablePointer&lt;UInt32>

A pointer to the first attribute tag in the array.

### Initializers

init(count: UInt32, tag: UnsafeMutablePointer&lt;UInt32>, format: UnsafeMutablePointer&lt;UInt32>?)

Creates a new attribute information structure.

## Relationships

### Conforms To

- BitwiseCopyable

