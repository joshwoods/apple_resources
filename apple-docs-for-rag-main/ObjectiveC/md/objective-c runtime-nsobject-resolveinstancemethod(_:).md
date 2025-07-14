

- Objective-C Runtime
- NSObject
-  resolveInstanceMethod(\_:) 

Type Method

# resolveInstanceMethod(\_:)

Dynamically provides an implementation for a given selector for an instance method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func resolveInstanceMethod(_ sel: Selector!) -> Bool
```

## Parameters 

`sel`  

The name of a selector to resolve.

## Return Value

YES if the method was found and added to the receiver, otherwise NO.

## Discussion

This method and resolveClassMethod(_:) allow you to dynamically provide an implementation for a given selector.

An Objective-C method is simply a C function that take at least two arguments—`self` and `_cmd`. Using the class_addMethod(_:_:_:_:) function, you can add a function to a class as a method. Given the following function:

```
void dynamicMethodIMP(id self, SEL _cmd)
{
    // implementation ....
}
```

you can use `resolveInstanceMethod:` to dynamically add it to a class as a method (called `resolveThisMethodDynamically`) like this:

```
+ (BOOL) resolveInstanceMethod:(SEL)aSEL
{
    if (aSEL == @selector(resolveThisMethodDynamically))
    {
          class_addMethod([self class], aSEL, (IMP) dynamicMethodIMP, "v@:");
          return YES;
    }
    return [super resolveInstanceMethod:aSel];
}
```

### Special Considerations

This method is called before the Objective-C forwarding mechanism is invoked. If responds(to:) or instancesRespond(to:) is invoked, the dynamic method resolver is given the opportunity to provide an `IMP` for the given selector first.

## See Also

### Dynamically Resolving Methods

class func resolveClassMethod(Selector!) -> Bool

Dynamically provides an implementation for a given selector for a class method.

