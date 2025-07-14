

- JavaScriptCore
- JSValue
-  objectForKeyedSubscript(\_:) 

Instance Method

# objectForKeyedSubscript(\_:)

Returns the value’s JavaScript property named with the specified key, allowing subscript syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func objectForKeyedSubscript(_ key: Any!) -> JSValue!
```

## Parameters 

`key`  

The name of a property in the JavaScript object.

## Return Value

The value of the named property, or the JavaScript `undefined` value if no property exists by that name.

## Discussion

This method is equivalent to the forProperty(_:) method, but provides Objective-C subscripting support.

## See Also

### Accessing Values with Subscript Syntax

func objectAtIndexedSubscript(Int) -> JSValue!

Returns the value’s JavaScript property at the specified index, allowing subscript syntax.

func setObject(Any!, atIndexedSubscript: Int)

Sets the value’s JavaScript property at the specified index, allowing subscript syntax.

func setObject(Any!, forKeyedSubscript: Any!)

Sets the value’s JavaScript property named with the specified key, allowing subscript syntax.

