

- Foundation
- NSProxy
-  forwardInvocation(\_:) 

Instance Method

# forwardInvocation(\_:)

Passes a given invocation to the real object the proxy represents.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func forwardInvocation(_ invocation: NSInvocation)
```

## Parameters 

`invocation`  

The invocation to forward.

## Discussion

`NSProxy`’s implementation merely raises `NSInvalidArgumentException`. Override this method in your subclass to handle `invocation` appropriately, at the very least by setting its return value.

For example, if your proxy merely forwards messages to an instance variable named `realObject`, it can implement forwardInvocation(_:) like this:

```
- (void)forwardInvocation:(NSInvocation *)anInvocation
{
    [anInvocation setTarget:realObject];
    [anInvocation invoke];
    return;
}
```

