

- Objective-C Runtime
- NSObject
-  instanceMethod(for:) 

Type Method

# instanceMethod(for:)

Locates and returns the address of the implementation of the instance method identified by a given selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func instanceMethod(for aSelector: Selector!) -> IMP!
```

## Parameters 

`aSelector`  

A Selector that identifies the method for which to return the implementation address. The selector must be non-`NULL` and valid for the receiver. If in doubt, use the responds(to:) method to check before passing the selector to method(for:).

## Return Value

The address of the implementation of the `aSelector` instance method.

## Discussion

An error is generated if instances of the receiver can’t respond to `aSelector` messages.

Use this method to ask the class object for the implementation of instance methods only. To ask the class for the implementation of a class method, send the method(for:) instance method to the class instead.

## See Also

### Obtaining Information About Methods

func method(for: Selector!) -> IMP!

Locates and returns the address of the receiver’s implementation of a method so it can be called as a function.

