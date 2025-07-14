

- Objective-C Runtime
- NSObject
-  autoContentAccessingProxy 

Instance Property

# autoContentAccessingProxy

A proxy for the receiving object

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var autoContentAccessingProxy: Any { get }
```

## Discussion

This property returns a proxy for the receiving object if the receiver adopts the NSDiscardableContent protocol and still has content that has not been discarded.

The proxy calls beginContentAccess() on the receiver to keep the content available as long as the proxy lives, and calls endContentAccess() when the proxy is deallocated.

The wrapper object is otherwise a subclass of NSProxy and forwards messages to the original receiver object as an NSProxy does.

This method can be used to hide an NSDiscardableContent object’s content volatility by creating an object that responds to the same messages but holds the contents of the original receiver available as long as the created proxy lives. Thus hidden, the NSDiscardableContent object (by way of the proxy) can be given out to unsuspecting recipients of the object who would otherwise not know they might have to call beginContentAccess() and endContentAccess() around particular usages (specific to each NSDiscardableContent object) of the NSDiscardableContent object.

