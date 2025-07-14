

- JavaScriptCore
- JSValue
-  isInstance(of:) 

Instance Method

# isInstance(of:)

Returns a Boolean value indicating whether the value is an instance of another JavaScript object value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func isInstance(of value: Any!) -> Bool
```

## Parameters 

`value`  

The value to be compared against.

## Return Value

true if this value inherits from `value`; otherwise, false.

## Discussion

This method is analogous to the `instanceof` operator in JavaScript: it tests for the presence of the specified value’s constructor prototype in this value’s prototype chain.

## See Also

### Comparing JavaScript Values

func isEqual(to: Any!) -> Bool

Compares the value to another for strict equality.

func isEqualWithTypeCoercion(to: Any!) -> Bool

Compares the value to another for equivalence, allowing type conversion.

