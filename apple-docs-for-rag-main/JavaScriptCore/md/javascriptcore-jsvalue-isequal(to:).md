

- JavaScriptCore
- JSValue
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Compares the value to another for strict equality.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func isEqual(to value: Any!) -> Bool
```

## Parameters 

`value`  

The value to be compared against.

## Return Value

true if the values are strictly equal; otherwise, false.

## Discussion

This method is analogous to the identity or strict equality operator `===` in JavaScript.

## See Also

### Comparing JavaScript Values

func isEqualWithTypeCoercion(to: Any!) -> Bool

Compares the value to another for equivalence, allowing type conversion.

func isInstance(of: Any!) -> Bool

Returns a Boolean value indicating whether the value is an instance of another JavaScript object value.

