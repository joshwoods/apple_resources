

- Foundation
- Object Runtime
-  Objective-C Runtime Utilities 

API Collection

# Objective-C Runtime Utilities

Interact with the Objective-C runtime.

## Topics

### Type Lookup

func NSClassFromString(String) -> AnyClass?

Obtains a class by name.

func NSStringFromClass(AnyClass) -> String

Returns the name of a class as a string.

func NSSelectorFromString(String) -> Selector

Returns the selector with a given name.

func NSStringFromSelector(Selector) -> String

Returns a string representation of a given selector.

func NSStringFromProtocol(Protocol) -> String

Returns the name of a protocol as a string.

func NSProtocolFromString(String) -> Protocol?

Returns a the protocol with a given name.

### Serialization

func NSGetSizeAndAlignment(UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?) -> UnsafePointer&lt;CChar>

Obtains the actual size and the aligned size of an encoded type.

