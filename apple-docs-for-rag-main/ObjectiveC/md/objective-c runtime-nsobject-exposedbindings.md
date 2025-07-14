

- Objective-C Runtime
- NSObject
-  exposedBindings 

Instance Property

# exposedBindings

Returns an array containing the bindings exposed by the receiver.

macOS

``` source
var exposedBindings: [NSBindingName] { get }
```

## Return Value

An array containing the bindings exposed by the receiver.

## Discussion

A subclass can override this method to remove bindings that are exposed by a superclass that are not appropriate for the subclass.

## See Also

### Exposing bindings

class func exposeBinding(NSBindingName)

Exposes the specified `binding`, advertising its availability.

