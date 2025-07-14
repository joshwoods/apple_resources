

- Swift
- Double
-  round(\_:) 

Instance Method

# round(\_:)

Rounds the value to an integral value using the specified rounding rule.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func round(_ rule: FloatingPointRoundingRule)
```

## Parameters 

`rule`  

The rounding rule to use.

## Discussion

The following example rounds a value using four different rounding rules:

```
// Equivalent to the C 'round' function:
var w = 6.5
w.round(.toNearestOrAwayFromZero)
// w == 7.0

// Equivalent to the C 'trunc' function:
var x = 6.5
x.round(.towardZero)
// x == 6.0

// Equivalent to the C 'ceil' function:
var y = 6.5
y.round(.up)
// y == 7.0

// Equivalent to the C 'floor' function:
var z = 6.5
z.round(.down)
// z == 6.0
```

For more information about the available rounding rules, see the `FloatingPointRoundingRule` enumeration. To round a value using the default “schoolbook rounding”, you can use the shorter `round()` method instead.

```
var w1 = 6.5
w1.round()
// w1 == 7.0
```

## See Also

### Rounding Values

func rounded() -> Self

func rounded(FloatingPointRoundingRule) -> Self

Returns this value rounded to an integral value using the specified rounding rule.

func round()

