

- Swift
- UInt32
-  random(in:) 

Type Method

# random(in:)

Returns a random value within the specified range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func random(in range: Range) -> Self
```

## Parameters 

`range`  

The range in which to create a random value. `range` must not be empty.

## Return Value

A random value within the bounds of `range`.

## Discussion

Use this method to generate an integer within a specific range. This example creates three new values in the range `1..

```
for _ in 1...3 {
    print(Int.random(in: 1..

This method is equivalent to calling the version that takes a generator, passing in the system’s default random generator.

