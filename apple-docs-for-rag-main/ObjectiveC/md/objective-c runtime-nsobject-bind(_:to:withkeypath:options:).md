

- Objective-C Runtime
- NSObject
-  bind(\_:to:withKeyPath:options:) 

Instance Method

# bind(\_:to:withKeyPath:options:)

Establishes a binding between a given property of the receiver and the property of a given object specified by a given key path.

macOS

``` source
func bind(
    _ binding: NSBindingName,
    to observable: Any,
    withKeyPath keyPath: String,
    options: [NSBindingOption : Any]? = nil
)
```

## Parameters 

`binding`  

The key path for a property of the receiver previously exposed using the exposeBinding(_:) method.

`observable`  

The bound-to object.

`keyPath`  

A key path to a property reachable from `observableController`. The elements in the path must be key-value observing compliant (see Key-Value Observing Programming Guide).

`options`  

A dictionary containing options for the binding, such as placeholder objects or an `NSValueTransformer` identifier as described in Constants. This value is optional—pass `nil` to specify no options.

## See Also

### Managing bindings

func valueClassForBinding(NSBindingName) -> AnyClass?

Returns the class of the value that will be returned for the specified binding.

func optionDescriptionsForBinding(NSBindingName) -> [NSAttributeDescription]

Returns an array describing the options for the specified binding.

func infoForBinding(NSBindingName) -> [NSBindingInfoKey : Any]?

Returns a dictionary describing the receiver’s `binding`.

struct NSBindingInfoKey

func unbind(NSBindingName)

Removes a given binding between the receiver and a controller.

func NSIsControllerMarker(_ object: Any?) -> Bool

Tests whether a given object is special marker object used for indicating the state of a selection in relation to a key.

