

- Swift
- Float
-  rounded(\_:) 

Instance Method

# rounded(\_:)

Returns this value rounded to an integral value using the specified rounding rule.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rounded(_ rule: FloatingPointRoundingRule) -> Self
```

## Parameters 

`rule`  

The rounding rule to use.

## Return Value

The integral value found by rounding using `rule`.

## Discussion

The following example rounds a value using four different rounding rules:

```
let x = 6.5

// Equivalent to the C 'round' function:
print(x.rounded(.toNearestOrAwayFromZero))
// Prints "7.0"

// Equivalent to the C 'trunc' function:
print(x.rounded(.towardZero))
// Prints "6.0"

// Equivalent to the C 'ceil' function:
print(x.rounded(.up))
// Prints "7.0"

// Equivalent to the C 'floor' function:
print(x.rounded(.down))
// Prints "6.0"
```

For more information about the available rounding rules, see the `FloatingPointRoundingRule` enumeration. To round a value using the default “schoolbook rounding”, you can use the shorter `rounded()` method instead.

```
print(x.rounded())
// Prints "7.0"
```

## See Also

### Rounding Values

func rounded() -> Self

func round()

func round(FloatingPointRoundingRule)

Rounds the value to an integral value using the specified rounding rule.

