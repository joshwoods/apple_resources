

- Objective-C Runtime
- NSObject
-  conforms(to:) 

Type Method

# conforms(to:)

Returns a Boolean value that indicates whether the target conforms to a given protocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func conforms(to protocol: Protocol) -> Bool
```

## Parameters 

`protocol`  

A protocol.

## Return Value

YES if the target conforms to `protocol`, otherwise NO.

## Discussion

A class “conforms to” a protocol if it adopts the protocol or inherits from another class that adopts it. Classes adopt protocols by listing them within angle brackets after the interface declaration. For example, here `MyClass` adopts the (fictitious) `AffiliationRequests` and `Normalization` protocols:

```
@interface MyClass : NSObject 
```

A class also conforms to any protocols included in the protocols it adopts or inherits. Protocols incorporate other protocols in the same way classes adopt them. For example, here the `AffiliationRequests` protocol incorporates the `Joining` protocol:

```
@protocol AffiliationRequests 
```

If a class adopts a protocol that incorporates another protocol, it must also implement all the methods in the incorporated protocol or inherit those methods from a class that adopts it.

This method determines conformance solely on the basis of the formal declarations in header files, as illustrated above. It doesn’t check to see whether the methods declared in the protocol are actually implemented—that’s the programmer’s responsibility.

To specify the protocol required as this method’s argument, use the `@protocol()` directive:

```
BOOL canJoin = [MyClass conformsToProtocol:@protocol(Joining)];
```

### Performance Considerations

Calling this method in performance sensitive code can cause unwanted performance problems. conforms(to:) requires taking the Objective-C runtime lock and traversing the target’s class hierarchy to check for protocol conformance, which can take significant time.

Consider the following alternatives in your code:

- Use responds(to:) to check for methods in the protocol instead, especially if you only need to check some of the protocol’s methods.

- If you do need to use conforms(to:), cache the result whenever possible, rather than calling this method repeatedly.

