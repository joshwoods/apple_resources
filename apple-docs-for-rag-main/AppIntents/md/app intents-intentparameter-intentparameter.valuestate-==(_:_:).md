

- App Intents
- IntentParameter
- IntentParameter.ValueState
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
static func == (lhs: IntentParameter.ValueState, rhs: IntentParameter.ValueState) -> Bool
```

Available when `Value` conforms to `_IntentValue`, `Equatable`, and `Sendable`.

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

