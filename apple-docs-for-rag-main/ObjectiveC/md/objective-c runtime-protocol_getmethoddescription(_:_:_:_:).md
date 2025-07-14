

- Objective-C Runtime
-  protocol_getMethodDescription(\_:\_:\_:\_:) 

Function

# protocol_getMethodDescription(\_:\_:\_:\_:)

Returns a method description structure for a specified method of a given protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func protocol_getMethodDescription(
    _ proto: Protocol,
    _ aSel: Selector,
    _ isRequiredMethod: Bool,
    _ isInstanceMethod: Bool
) -> objc_method_description
```

## Parameters 

`proto`  

A protocol.

`aSel`  

A selector

`isRequiredMethod`  

A Boolean value that indicates whether `aSel` is a required method.

`isInstanceMethod`  

A Boolean value that indicates whether `aSel` is an instance method.

## Return Value

An `objc_method_description` structure that describes the method specified by `aSel`, `isRequiredMethod`, and `isInstanceMethod` for the protocol `p`.

## Discussion

If the protocol does not contain the specified method, returns an `objc_method_description` structure with the value `{NULL, NULL}`.

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

func protocol_copyPropertyList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_t>?

Returns an array of the properties declared by a protocol.

func protocol_getProperty(Protocol, UnsafePointer&lt;CChar>, Bool, Bool) -> objc_property_t?

Returns the specified property of a given protocol.

func protocol_copyProtocolList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of the protocols adopted by a protocol.

func protocol_conformsToProtocol(Protocol?, Protocol?) -> Bool

Returns a Boolean value that indicates whether one protocol conforms to another protocol.

