

- JavaScriptCore
- JSValue
-  setObject(\_:forKeyedSubscript:) 

Instance Method

# setObject(\_:forKeyedSubscript:)

Sets the value’s JavaScript property named with the specified key, allowing subscript syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func setObject(
    _ object: Any!,
    forKeyedSubscript key: Any!
)
```

## Parameters 

`object`  

The value to set for the named JavaScript property.

`key`  

The name of a property in the JavaScript object.

## Discussion

This method is equivalent to the setValue(_:forProperty:) method, but provides Objective-C subscripting support.

## See Also

### Accessing Values with Subscript Syntax

func objectAtIndexedSubscript(Int) -> JSValue!

Returns the value’s JavaScript property at the specified index, allowing subscript syntax.

func setObject(Any!, atIndexedSubscript: Int)

Sets the value’s JavaScript property at the specified index, allowing subscript syntax.

func objectForKeyedSubscript(Any!) -> JSValue!

Returns the value’s JavaScript property named with the specified key, allowing subscript syntax.

