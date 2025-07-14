

- Objective-C Runtime
- NSObjectProtocol
-  conforms(to:) 

Instance Method

# conforms(to:)

Returns a Boolean value that indicates whether the receiver conforms to a given protocol.

iOSiPadOSMac Catalyst 13.1+macOS 10.0+tvOSvisionOSwatchOS

``` source
func conforms(to aProtocol: Protocol) -> Bool
```

**Required**

## Parameters 

`aProtocol`  

A protocol object that represents a particular protocol.

## Return Value

YES if the receiver conforms to `aProtocol`, otherwise NO.

## Discussion

This method works identically to the conforms(to:) class method declared in NSObject. It’s provided as a convenience so that you don’t need to get the class object to find out whether an instance can respond to a given set of messages.

## See Also

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

