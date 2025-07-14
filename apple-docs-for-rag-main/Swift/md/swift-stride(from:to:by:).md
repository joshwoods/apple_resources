

- Swift
-  stride(from:to:by:) 

Function

# stride(from:to:by:)

Returns a sequence from a starting value to, but not including, an end value, stepping by the specified amount.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func stride(
    from start: T,
    to end: T,
    by stride: T.Stride
) -> StrideTo where T : Strideable
```

## Parameters 

`start`  

The starting value to use for the sequence. If the sequence contains any values, the first one is `start`.

`end`  

An end value to limit the sequence. `end` is never an element of the resulting sequence.

`stride`  

The amount to step by with each iteration. A positive `stride` iterates upward; a negative `stride` iterates downward.

## Return Value

A sequence from `start` toward, but not including, `end`. Each value in the sequence steps by `stride`.

## Discussion

You can use this function to stride over values of any type that conforms to the `Strideable` protocol, such as integers or floating-point types. Starting with `start`, each successive value of the sequence adds `stride` until the next value would be equal to or beyond `end`.

```
for radians in stride(from: 0.0, to: .pi * 2, by: .pi / 2) {
    let degrees = Int(radians * 180 / .pi)
    print("Degrees: \(degrees), radians: \(radians)")
}
// Degrees: 0, radians: 0.0
// Degrees: 90, radians: 1.5707963267949
// Degrees: 180, radians: 3.14159265358979
// Degrees: 270, radians: 4.71238898038469
```

You can use `stride(from:to:by:)` to create a sequence that strides upward or downward. Pass a negative value as `stride` to create a sequence from a higher start to a lower end:

```
for countdown in stride(from: 3, to: 0, by: -1) {
    print("\(countdown)...")
}
// 3...
// 2...
// 1...
```

If you pass a value as `stride` that moves away from `end`, the sequence contains no values.

```
for x in stride(from: 0, to: 10, by: -1) {
    print(x)
}
// Nothing is printed.
```

## See Also

### Strides

func stride&lt;T>(from: T, through: T, by: T.Stride) -> StrideThrough&lt;T>

Returns a sequence from a starting value toward, and possibly including, an end value, stepping by the specified amount.

