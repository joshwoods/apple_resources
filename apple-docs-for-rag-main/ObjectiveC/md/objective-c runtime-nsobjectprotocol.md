

- Objective-C Runtime
-  NSObjectProtocol 

Protocol

# NSObjectProtocol

The group of methods that are fundamental to all Objective-C objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol NSObjectProtocol
```

## Overview

Note

This protocol is imported into Swift with the name `NSObjectProtocol`.

An object that conforms to this protocol can be considered a first-class object. Such an object can be asked about its:

- Class, and the place of its class in the inheritance hierarchy.

- Conformance to protocols.

- Ability to respond to a particular message.

The Cocoa root class NSObject adopts this protocol, so all objects inheriting from NSObject have the features described by this protocol.

## Topics

### Identifying Classes

var superclass: AnyClass?

Returns the class object for the receiver’s superclass.

**Required**

### Identifying and Comparing Objects

func isEqual(Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

**Required**

var hash: Int

Returns an integer that can be used as a table address in a hash table structure.

**Required**

func `self`() -> Self

Returns the receiver.

**Required**

### Testing Object Inheritance, Behavior, and Conformance

func isKind(of: AnyClass) -> Bool

Returns a Boolean value that indicates whether the receiver is an instance of given class or an instance of any class that inherits from that class.

**Required**

func isMember(of: AnyClass) -> Bool

Returns a Boolean value that indicates whether the receiver is an instance of a given class.

**Required**

func responds(to: Selector!) -> Bool

Returns a Boolean value that indicates whether the receiver implements or inherits a method that can respond to a specified message.

**Required**

func conforms(to: Protocol) -> Bool

Returns a Boolean value that indicates whether the receiver conforms to a given protocol.

**Required**

### Describing Objects

var description: String

A textual representation of the receiver.

**Required**

var debugDescription: String

A textual representation of the receiver to use with a debugger.

### Sending Messages

func perform(Selector!) -> Unmanaged&lt;AnyObject>!

Sends a specified message to the receiver and returns the result of the message.

**Required**

func perform(Selector!, with: Any!) -> Unmanaged&lt;AnyObject>!

Sends a message to the receiver with an object as the argument.

**Required**

func perform(Selector!, with: Any!, with: Any!) -> Unmanaged&lt;AnyObject>!

Sends a message to the receiver with two objects as arguments.

**Required**

### Identifying Proxies

func isProxy() -> Bool

Returns a Boolean value that indicates whether the receiver does not descend from NSObject.

**Required**

## Relationships

### Conforming Types

- NSObject

