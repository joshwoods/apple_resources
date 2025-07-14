

- JavaScriptCore
- JSValue
-  hasProperty(\_:) 

Instance Method

# hasProperty(\_:)

Returns a Boolean value indicating whether the JavaScript value has a defined property with the specified name.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

**tvOS**

``` source
func hasProperty(_ property: String!) -> Bool
```

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func hasProperty(_ property: Any!) -> Bool
```

## Parameters 

`property`  

The name of a property to query for in the JavaScript object value.

## Return Value

true if the JavaScript object has a defined property by that name; otherwise, false.

## See Also

### Working with Container Values

func defineProperty(Any!, descriptor: Any!)

Defines a property on the JavaScript object value or modifies a property’s definition.

func deleteProperty(Any!) -> Bool

Deletes the named property from the JavaScript object value.

func atIndex(Int) -> JSValue!

Returns the value at the specified numeric index in the JavaScript object value.

func setValue(Any!, at: Int)

Sets the value at the specified numeric index in the JavaScript object value.

func forProperty(Any!) -> JSValue!

Returns the value of the named property in the JavaScript object value.

func setValue(Any!, forProperty: Any!)

Sets the value of the named property in the JavaScript object value.

typealias JSValueProperty

A type that identifies a property of a JavaScript value.

