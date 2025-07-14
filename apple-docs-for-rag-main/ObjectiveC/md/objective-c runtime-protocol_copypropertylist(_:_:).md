

- Objective-C Runtime
-  protocol_copyPropertyList(\_:\_:) 

Function

# protocol_copyPropertyList(\_:\_:)

Returns an array of the properties declared by a protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func protocol_copyPropertyList(
    _ proto: Protocol,
    _ outCount: UnsafeMutablePointer?
) -> UnsafeMutablePointer?
```

## Parameters 

`proto`  

A protocol.

`outCount`  

Upon return, contains the number of elements in the returned array.

## Return Value

A C array of pointers of type `objc_property_t` describing the properties declared by `proto`. Any properties declared by other protocols adopted by this protocol are not included. The array contains `*outCount` pointers followed by a `NULL` terminator. You must free the array with `free()`.

## Discussion

If the protocol declares no properties, `NULL` is returned and `*outCount` is `0`.

## See Also

### Working with Protocols

func objc_getProtocol(UnsafePointer&lt;CChar>) -> Protocol?

Returns a specified protocol.

func objc_copyProtocolList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of all the protocols known to the runtime.

func objc_allocateProtocol(UnsafePointer&lt;CChar>) -> Protocol?

Creates a new protocol instance.

func objc_registerProtocol(Protocol)

Registers a newly created protocol with the Objective-C runtime.

func protocol_addMethodDescription(Protocol, Selector, UnsafePointer&lt;CChar>?, Bool, Bool)

Adds a method to a protocol.

func protocol_addProtocol(Protocol, Protocol)

Adds a registered protocol to another protocol that is under construction.

func protocol_addProperty(Protocol, UnsafePointer&lt;CChar>, UnsafePointer&lt;objc_property_attribute_t>?, UInt32, Bool, Bool)

Adds a property to a protocol that is under construction.

func protocol_getName(Protocol) -> UnsafePointer&lt;CChar>

Returns the name of a protocol.

func protocol_isEqual(Protocol?, Protocol?) -> Bool

Returns a Boolean value that indicates whether two protocols are equal.

func protocol_copyMethodDescriptionList(Protocol, Bool, Bool, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_method_description>?

Returns an array of method descriptions of methods meeting a given specification for a given protocol.

func protocol_getMethodDescription(Protocol, Selector, Bool, Bool) -> objc_method_description

Returns a method description structure for a specified method of a given protocol.

func protocol_getProperty(Protocol, UnsafePointer&lt;CChar>, Bool, Bool) -> objc_property_t?

Returns the specified property of a given protocol.

func protocol_copyProtocolList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of the protocols adopted by a protocol.

func protocol_conformsToProtocol(Protocol?, Protocol?) -> Bool

Returns a Boolean value that indicates whether one protocol conforms to another protocol.

