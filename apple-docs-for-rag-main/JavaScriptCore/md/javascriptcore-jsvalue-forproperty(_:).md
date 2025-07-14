

- JavaScriptCore
- JSValue
-  forProperty(\_:) 

Instance Method

# forProperty(\_:)

Returns the value of the named property in the JavaScript object value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func forProperty(_ property: Any!) -> JSValue!
```

**tvOS**

``` source
func forProperty(_ property: String!) -> JSValue!
```

## Parameters 

`property`  

The name of a property in the JavaScript object.

## Return Value

The value of the named property, or the JavaScript `undefined` value if no property exists by that name.

## Discussion

Calling this method is equivalent to using the subscript operator with a string subscript in JavaScript. Use it to access fields or properties in JavaScript objects.

## Topics

### Related Documentation

func objectForKeyedSubscript(Any!) -> JSValue!

Returns the value’s JavaScript property named with the specified key, allowing subscript syntax.

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

func setValue(Any!, at: Int)

Sets the value at the specified numeric index in the JavaScript object value.

func setValue(Any!, forProperty: Any!)

Sets the value of the named property in the JavaScript object value.

typealias JSValueProperty

A type that identifies a property of a JavaScript value.

