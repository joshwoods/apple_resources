

- JavaScriptCore
- JSValue
-  deleteProperty(\_:) 

Instance Method

# deleteProperty(\_:)

Deletes the named property from the JavaScript object value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func deleteProperty(_ property: Any!) -> Bool
```

**tvOS**

``` source
func deleteProperty(_ property: String!) -> Bool
```

## Parameters 

`property`  

The name of a property in the JavaScript object value.

## Return Value

true if property deletion was successful; otherwise, false.

## Discussion

Calling this method is equivalent to using the JavaScript `delete` operator on an object (for example, `delete object.property`). After deletion, attempting to retrieve the property’s value results in the undefined value, and any descriptor information that defines the property’s behavior (see the defineProperty(_:descriptor:) method or the JavaScript `defineProperty` function) is lost.

## See Also

### Working with Container Values

func defineProperty(Any!, descriptor: Any!)

Defines a property on the JavaScript object value or modifies a property’s definition.

func hasProperty(Any!) -> Bool

Returns a Boolean value indicating whether the JavaScript value has a defined property with the specified name.

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

