

- JavaScriptCore
- JSValue
-  Property Descriptor Keys 

API Collection

# Property Descriptor Keys

Keys for the native dictionary representation of a JavaScript property descriptor, used with the defineProperty(_:descriptor:) method.

## Topics

### Constants

let JSPropertyDescriptorWritableKey: String

The Boolean value for this key determines whether the property permits assignment with the JavaScript `=` operator.

let JSPropertyDescriptorEnumerableKey: String

The Boolean value for this key determines whether the property appears when enumerating the JavaScript object’s properties.

let JSPropertyDescriptorConfigurableKey: String

The Boolean value for this key determines whether the property deleted from its JavaScript object or its descriptor changed.

let JSPropertyDescriptorValueKey: String

The value for the property on the JavaScript object.

let JSPropertyDescriptorGetKey: String

The JavaScript function to be invoked when reading the property.

let JSPropertyDescriptorSetKey: String

The JavaScript function to be invoked when writing to the property.

