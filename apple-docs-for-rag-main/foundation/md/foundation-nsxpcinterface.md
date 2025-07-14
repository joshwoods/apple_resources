

- Foundation
-  NSXPCInterface 

Class

# NSXPCInterface

An interface that may be sent to an exported object or remote object proxy.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSXPCInterface
```

## Overview

This object holds all information about the interface of an exported object or remote object proxy. It describes what messages are allowed, what kinds of objects are allowed as arguments, what the signature of any reply blocks are, and information about additional proxy objects.

## Topics

### Initializers

init(with: Protocol)

Returns an NSXPCInterface instance for a given protocol.

### Instance Properties

var `protocol`: Protocol

The Objective-C protocol that this interface is based on.

### Instance Methods

func classes(for: Selector, argumentIndex: Int, ofReply: Bool) -> Set&lt;AnyHashable>

Returns the current list of allowed classes that can appear within the specified collection object argument to the specified method.

func forSelector(Selector, argumentIndex: Int, ofReply: Bool) -> NSXPCInterface?

Returns the interface previously set for the specified selector and parameter.

func setClasses(Set&lt;AnyHashable>, for: Selector, argumentIndex: Int, ofReply: Bool)

Sets the classes that can appear within the (numerically) specified collection object argument to the specified method.

func setInterface(NSXPCInterface, for: Selector, argumentIndex: Int, ofReply: Bool)

Configures a specific parameter of a method to be sent as a proxy object instead of copied.

func setXPCType(xpc_type_t, for: Selector, argumentIndex: Int, ofReply: Bool)

func xpcType(for: Selector, argumentIndex: Int, ofReply: Bool) -> xpc_type_t?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### XPC Client

protocol NSXPCProxyCreating

Methods for creating new proxy objects.

class NSXPCConnection

A bidirectional communication channel between two processes.

class NSXPCCoder

A coder that encodes and decodes objects that your app sends over an XPC connection.

