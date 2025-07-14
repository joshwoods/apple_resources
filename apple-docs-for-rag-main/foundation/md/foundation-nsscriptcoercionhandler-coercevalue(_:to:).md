

- Foundation
- NSScriptCoercionHandler
-  coerceValue(\_:to:) 

Instance Method

# coerceValue(\_:to:)

Returns an object of a given class representing a given value.

Mac Catalyst 13.0+macOS 10.0+

``` source
func coerceValue(
    _ value: Any,
    to toClass: AnyClass
) -> Any?
```

## Parameters 

`value`  

The value to coerce.

`toClass`  

The class with which to represent `value`.

## Return Value

An object of the class `toClass` representing the value specified by `value`. Returns `nil` if an error occurs.

## See Also

### Working with handlers

func registerCoercer(Any, selector: Selector, toConvertFrom: AnyClass, to: AnyClass)

Registers a given object (typically a class) to handle coercions (conversions) from one given class to another.

