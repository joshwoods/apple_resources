

- Foundation
-  NSProxy 

Class

# NSProxy

An abstract superclass defining an API for objects that act as stand-ins for other objects or for objects that don’t exist yet.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSProxy
```

## Overview

Typically, a message to a proxy is forwarded to the real object or causes the proxy to load (or transform itself into) the real object. Subclasses of NSProxy can be used to implement transparent distributed messaging (for example, NSDistantObject) or for lazy instantiation of objects that are expensive to create.

NSProxy implements the basic methods required of a root class, including those defined in the NSObjectProtocol protocol. However, as an abstract class it doesn’t provide an initialization method, and it raises an exception upon receiving any message it doesn’t respond to. A concrete subclass must therefore provide an initialization or creation method and override the forwardInvocation(_:) and methodSignatureForSelector: methods to handle messages that it doesn’t implement itself. A subclass’s implementation of forwardInvocation(_:) should do whatever is needed to process the invocation, such as forwarding the invocation over the network or loading the real object and passing it the invocation. methodSignatureForSelector: is required to provide argument type information for a given message; a subclass’s implementation should be able to determine the argument types for the messages it needs to forward and should construct an NSMethodSignature object accordingly. See the NSDistantObject, NSInvocation, and NSMethodSignature class specifications for more information.

## Topics

### Creating Instances

class func alloc() -> Self

Returns a new instance of the receiving class

### Deallocating Instances

func dealloc()

Deallocates the memory occupied by the receiver.

### Finalizing an Object

func finalize()

The garbage collector invokes this method on the receiver before disposing of the memory it uses.

### Handling Unimplemented Methods

func forwardInvocation(NSInvocation)

Passes a given invocation to the real object the proxy represents.

### Introspecting a Proxy Class

class func responds(to: Selector) -> Bool

Returns a Boolean value that indicates whether the receiving class responds to a given selector.

### Describing a Proxy Class or Object

class func `class`() -> AnyClass

Returns `self` (the class object).

var description: String

var debugDescription: String

## Relationships

### Inherited By

- NSProtocolChecker

### Conforms To

- NSObjectProtocol

