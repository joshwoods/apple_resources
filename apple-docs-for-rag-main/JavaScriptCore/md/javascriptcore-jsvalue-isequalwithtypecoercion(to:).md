

- JavaScriptCore
- JSValue
-  isEqualWithTypeCoercion(to:) 

Instance Method

# isEqualWithTypeCoercion(to:)

Compares the value to another for equivalence, allowing type conversion.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func isEqualWithTypeCoercion(to value: Any!) -> Bool
```

## Parameters 

`value`  

The value to be compared against.

## Return Value

true if the values are equivalent; otherwise, false.

## Discussion

This method is analogous to the equality operator `==` in JavaScript: it first converts its operands to the same type (if they are not already of the same type), then applies a strict equality comparison to the result. JavaScript object values are equal if and only if they refer to the same object instance.

## See Also

### Comparing JavaScript Values

func isEqual(to: Any!) -> Bool

Compares the value to another for strict equality.

func isInstance(of: Any!) -> Bool

Returns a Boolean value indicating whether the value is an instance of another JavaScript object value.

