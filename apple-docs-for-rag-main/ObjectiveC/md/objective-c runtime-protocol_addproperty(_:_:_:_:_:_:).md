

- Objective-C Runtime
-  protocol_addProperty(\_:\_:\_:\_:\_:\_:) 

Function

# protocol_addProperty(\_:\_:\_:\_:\_:\_:)

Adds a property to a protocol that is under construction.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func protocol_addProperty(
    _ proto: Protocol,
    _ name: UnsafePointer,
    _ attributes: UnsafePointer?,
    _ attributeCount: UInt32,
    _ isRequiredProperty: Bool,
    _ isInstanceProperty: Bool
)
```

## Parameters 

`proto`  

The protocol you want to add a property to.

`name`  

The name of the property you want to add.

`attributes`  

An array of property attributes.

`attributeCount`  

The number of properties in `attributes`.

`isRequiredProperty`  

A Boolean indicating whether the property’s accessor methods are required methods of the `proto` protocol. If YES, the property’s accessor methods are required methods; if NO, the property’s accessor methods are optional methods.

`isInstanceProperty`  

A Boolean indicating whether the property’s accessor methods are instance methods. If YES, the property’s accessor methods are instance methods. YES is the only value allowed for a property. As a result, if you set this value to NO, the property will not be added to the protocol.

## Discussion

The protocol you want to add the property to must be under construction—allocated but not yet registered with the Objective-C runtime (via the objc_registerProtocol(_:) function).

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

