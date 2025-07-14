

- Objective-C Runtime
- NSObjectProtocol
-  perform(\_:with:with:) 

Instance Method

# perform(\_:with:with:)

Sends a message to the receiver with two objects as arguments.

iOS 1.0+iPadOS 1.0+Mac Catalyst 1.0+macOS 10.0+tvOS 1.0+visionOS 1.0+watchOS 1.0+

``` source
func perform(
    _ aSelector: Selector!,
    with object1: Any!,
    with object2: Any!
) -> Unmanaged!
```

**Required**

## Parameters 

`aSelector`  

A selector identifying the message to send. If `aSelector` is `NULL`, an invalidArgumentException is raised.

`object1`  

An object that is the first argument of the message.

`object2`  

An object that is the second argument of the message

## Return Value

An object that is the result of the message.

## Discussion

This method is the same as perform(_:) except that you can supply two arguments for `aSelector`. `aSelector` should identify a method that can take two arguments of type id. For methods with other argument types and return values, use NSInvocation.

## See Also

### Related Documentation

func method(for: Selector!) -> IMP!

Locates and returns the address of the receiver’s implementation of a method so it can be called as a function.

### Sending Messages

func perform(Selector!) -> Unmanaged&lt;AnyObject>!

Sends a specified message to the receiver and returns the result of the message.

**Required**

func perform(Selector!, with: Any!) -> Unmanaged&lt;AnyObject>!

Sends a message to the receiver with an object as the argument.

**Required**

