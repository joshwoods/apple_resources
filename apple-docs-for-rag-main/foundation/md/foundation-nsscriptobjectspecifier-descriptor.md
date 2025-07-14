

- Foundation
- NSScriptObjectSpecifier
-  descriptor 

Instance Property

# descriptor

Returns an Apple event descriptor that represents the receiver.

macOS 10.5+

``` source
@NSCopying
var descriptor: NSAppleEventDescriptor? { get }
```

## Return Value

An Apple event descriptor of type `typeObjectSpecifier`.

## Discussion

If the receiver was created with init(descriptor:), the passed-in descriptor is returned. Otherwise, a new descriptor is created and returned, autoreleased.

