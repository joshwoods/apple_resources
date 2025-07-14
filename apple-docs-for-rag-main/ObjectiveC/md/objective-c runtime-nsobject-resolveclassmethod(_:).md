

- Objective-C Runtime
- NSObject
-  resolveClassMethod(\_:) 

Type Method

# resolveClassMethod(\_:)

Dynamically provides an implementation for a given selector for a class method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func resolveClassMethod(_ sel: Selector!) -> Bool
```

## Parameters 

`sel`  

The name of a selector to resolve.

## Return Value

YES if the method was found and added to the receiver, otherwise NO.

## Discussion

This method allows you to dynamically provide an implementation for a given selector. See resolveInstanceMethod(_:) for further discussion.

## See Also

### Dynamically Resolving Methods

class func resolveInstanceMethod(Selector!) -> Bool

Dynamically provides an implementation for a given selector for an instance method.

