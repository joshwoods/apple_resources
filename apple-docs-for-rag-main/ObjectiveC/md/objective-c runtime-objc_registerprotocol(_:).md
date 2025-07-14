

- Objective-C Runtime
-  objc_registerProtocol(\_:) 

Function

# objc_registerProtocol(\_:)

Registers a newly created protocol with the Objective-C runtime.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_registerProtocol(_ proto: Protocol)
```

## Parameters 

`proto`  

The protocol you want to register with the Objective-C runtime.

## Discussion

When you create a new protocol using the objc_allocateProtocol(_:), you then register it with the Objective-C runtime by calling this function. After a protocol is successfully registered, it is immutable and ready to use.

## See Also

### Working with Protocols

func objc_getProtocol(UnsafePointer&lt;CChar>) -> Protocol?

Returns a specified protocol.

func objc_copyProtocolList(UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of all the protocols known to the runtime.

func objc_allocateProtocol(UnsafePointer&lt;CChar>) -> Protocol?

Creates a new protocol instance.

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

func protocol_copyPropertyList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_t>?

Returns an array of the properties declared by a protocol.

func protocol_getProperty(Protocol, UnsafePointer&lt;CChar>, Bool, Bool) -> objc_property_t?

Returns the specified property of a given protocol.

func protocol_copyProtocolList(Protocol, UnsafeMutablePointer&lt;UInt32>?) -> AutoreleasingUnsafeMutablePointer&lt;Protocol>?

Returns an array of the protocols adopted by a protocol.

func protocol_conformsToProtocol(Protocol?, Protocol?) -> Bool

Returns a Boolean value that indicates whether one protocol conforms to another protocol.

