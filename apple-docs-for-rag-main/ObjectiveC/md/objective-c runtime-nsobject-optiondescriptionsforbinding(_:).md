

- Objective-C Runtime
- NSObject
-  optionDescriptionsForBinding(\_:) 

Instance Method

# optionDescriptionsForBinding(\_:)

Returns an array describing the options for the specified binding.

macOS 10.5+

``` source
func optionDescriptionsForBinding(_ binding: NSBindingName) -> [NSAttributeDescription]
```

## Parameters 

`binding`  

The name of a binding

## Return Value

Returns an array of NSAttributeDescription that describe the options for `binding`.

## Discussion

The NSAttributeDescription instances in the array are used by Interface Builder to build the options editor user interface of the bindings inspector.

- The option name displayed for the option in the bindings inspector is based on the value of the NSAttributeDescription method name.

- The type of editor displayed for the option in the bindings inspector is based on the value of the NSAttributeDescription method attributeType.

- The default value displayed in the bindings inspector for the option is based on the value of the NSAttributeDescription method defaultValue.

## See Also

### Managing bindings

func valueClassForBinding(NSBindingName) -> AnyClass?

Returns the class of the value that will be returned for the specified binding.

func bind(NSBindingName, to: Any, withKeyPath: String, options: [NSBindingOption : Any]?)

Establishes a binding between a given property of the receiver and the property of a given object specified by a given key path.

func infoForBinding(NSBindingName) -> [NSBindingInfoKey : Any]?

Returns a dictionary describing the receiver’s `binding`.

struct NSBindingInfoKey

func unbind(NSBindingName)

Removes a given binding between the receiver and a controller.

func NSIsControllerMarker(_ object: Any?) -> Bool

Tests whether a given object is special marker object used for indicating the state of a selection in relation to a key.

