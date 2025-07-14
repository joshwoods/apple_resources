

- Objective-C Runtime
- NSObject
-  valueClassForBinding(\_:) 

Instance Method

# valueClassForBinding(\_:)

Returns the class of the value that will be returned for the specified binding.

macOS

``` source
func valueClassForBinding(_ binding: NSBindingName) -> AnyClass?
```

## Parameters 

`binding`  

The name of a binding.

## Return Value

The class of the value that will be returned for `binding`.

## Discussion

This method is used by Interface Builder to determine the appropriate transformers for a binding.

Implementation of this method is optional.

## See Also

### Managing bindings

func bind(NSBindingName, to: Any, withKeyPath: String, options: [NSBindingOption : Any]?)

Establishes a binding between a given property of the receiver and the property of a given object specified by a given key path.

func optionDescriptionsForBinding(NSBindingName) -> [NSAttributeDescription]

Returns an array describing the options for the specified binding.

func infoForBinding(NSBindingName) -> [NSBindingInfoKey : Any]?

Returns a dictionary describing the receiver’s `binding`.

struct NSBindingInfoKey

func unbind(NSBindingName)

Removes a given binding between the receiver and a controller.

func NSIsControllerMarker(_ object: Any?) -> Bool

Tests whether a given object is special marker object used for indicating the state of a selection in relation to a key.

