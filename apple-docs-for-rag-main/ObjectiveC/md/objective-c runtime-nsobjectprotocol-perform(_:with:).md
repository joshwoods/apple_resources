

- Objective-C Runtime
- NSObjectProtocol
-  perform(\_:with:) 

Instance Method

# perform(\_:with:)

Sends a message to the receiver with an object as the argument.

iOS 1.0+iPadOS 1.0+Mac Catalyst 1.0+macOS 10.0+tvOS 1.0+visionOS 1.0+watchOS 1.0+

``` source
func perform(
    _ aSelector: Selector!,
    with object: Any!
) -> Unmanaged!
```

**Required**

## Parameters 

`aSelector`  

A selector identifying the message to send. If `aSelector` is `NULL`, an invalidArgumentException is raised.

`object`  

An object that is the sole argument of the message.

## Return Value

An object that is the result of the message.

## Discussion

This method is the same as perform(_:) except that you can supply an argument for `aSelector`. `aSelector` should identify a method that takes a single argument of type id. For methods with other argument types and return values, use NSInvocation.

## See Also

### Related Documentation

func method(for: Selector!) -> IMP!

Locates and returns the address of the receiver’s implementation of a method so it can be called as a function.

### Sending Messages

func perform(Selector!) -> Unmanaged&lt;AnyObject>!

Sends a specified message to the receiver and returns the result of the message.

**Required**

func perform(Selector!, with: Any!, with: Any!) -> Unmanaged&lt;AnyObject>!

Sends a message to the receiver with two objects as arguments.

**Required**

