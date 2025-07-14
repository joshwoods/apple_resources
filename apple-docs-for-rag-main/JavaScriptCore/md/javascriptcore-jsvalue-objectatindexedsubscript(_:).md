

- JavaScriptCore
- JSValue
-  objectAtIndexedSubscript(\_:) 

Instance Method

# objectAtIndexedSubscript(\_:)

Returns the value’s JavaScript property at the specified index, allowing subscript syntax.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func objectAtIndexedSubscript(_ index: Int) -> JSValue!
```

## Parameters 

`index`  

An index in the JavaScript object.

## Return Value

The value at the specified index, or the JavaScript `undefined` value if no property exists at that index.

## Discussion

This method is equivalent to the atIndex(_:) method, but provides Objective-C subscripting support.

## See Also

### Accessing Values with Subscript Syntax

func setObject(Any!, atIndexedSubscript: Int)

Sets the value’s JavaScript property at the specified index, allowing subscript syntax.

func objectForKeyedSubscript(Any!) -> JSValue!

Returns the value’s JavaScript property named with the specified key, allowing subscript syntax.

func setObject(Any!, forKeyedSubscript: Any!)

Sets the value’s JavaScript property named with the specified key, allowing subscript syntax.

