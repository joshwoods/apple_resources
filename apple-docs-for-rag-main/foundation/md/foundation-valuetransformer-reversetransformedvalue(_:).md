

- Foundation
- ValueTransformer
-  reverseTransformedValue(\_:) 

Instance Method

# reverseTransformedValue(\_:)

Returns the result of the reverse transformation of a given value.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func reverseTransformedValue(_ value: Any?) -> Any?
```

## Parameters 

`value`  

The value to reverse transform.

## Return Value

The reverse transformation of `value`.

## Discussion

The default implementation raises an exception if allowsReverseTransformation() returns false; otherwise it will invoke transformedValue(_:) with `value`.

A subclass should override this method if they require a reverse transformation that is not the same as simply reapplying the original transform (as would be the case with negation, for example). For example, if a value transformer converts a value in Fahrenheit to Celsius, this method would converts a value from Celsius to Fahrenheit.

## See Also

### Transforming Values

func transformedValue(Any?) -> Any?

Returns the result of transforming a given value.

