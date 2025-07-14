

- JavaScriptCore
- JSValue
-  setValue(\_:at:) 

Instance Method

# setValue(\_:at:)

Sets the value at the specified numeric index in the JavaScript object value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func setValue(
    _ value: Any!,
    at index: Int
)
```

## Parameters 

`value`  

The value to set at the specified index.

`index`  

An index in the JavaScript object.

## Discussion

Calling this method is equivalent to using the subscript operator with a numeric subscript in JavaScript. Use it to access elements of JavaScript arrays or of objects with numerically-indexed properties.

## Topics

### Related Documentation

func setObject(Any!, atIndexedSubscript: Int)

Sets the value’s JavaScript property at the specified index, allowing subscript syntax.

## See Also

### Working with Container Values

func defineProperty(Any!, descriptor: Any!)

Defines a property on the JavaScript object value or modifies a property’s definition.

func hasProperty(Any!) -> Bool

Returns a Boolean value indicating whether the JavaScript value has a defined property with the specified name.

func deleteProperty(Any!) -> Bool

Deletes the named property from the JavaScript object value.

func atIndex(Int) -> JSValue!

Returns the value at the specified numeric index in the JavaScript object value.

func forProperty(Any!) -> JSValue!

Returns the value of the named property in the JavaScript object value.

func setValue(Any!, forProperty: Any!)

Sets the value of the named property in the JavaScript object value.

typealias JSValueProperty

A type that identifies a property of a JavaScript value.

