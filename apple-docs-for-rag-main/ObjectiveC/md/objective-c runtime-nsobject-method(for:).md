

- Objective-C Runtime
- NSObject
-  method(for:) 

Instance Method

# method(for:)

Locates and returns the address of the receiver’s implementation of a method so it can be called as a function.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func method(for aSelector: Selector!) -> IMP!
```

## Parameters 

`aSelector`  

A Selector that identifies the method for which to return the implementation address. The selector must be a valid and non-`NULL`. If in doubt, use the responds(to:) method to check before passing the selector to method(for:).

## Return Value

The address of the receiver’s implementation of the `aSelector`.

## Discussion

If the receiver is an instance, `aSelector` should refer to an instance method; if the receiver is a class, it should refer to a class method.

## See Also

### Obtaining Information About Methods

class func instanceMethod(for: Selector!) -> IMP!

Locates and returns the address of the implementation of the instance method identified by a given selector.

