

- GameplayKit
- GKRandom
-  nextInt() 

Instance Method

# nextInt()

Generates and returns a new random integer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextInt() -> Int
```

**Required**

## Return Value

A random integer value in the range `[INT32_MIN, INT32_MAX]`.

## Discussion

For more information, see GameplayKit Programming Guide.

## See Also

### Generating Random Numbers

func nextInt(upperBound: Int) -> Int

Generates and returns a new random integer less than the specified limit.

**Required**

func nextUniform() -> Float

Generates and returns a new random floating-point value.

**Required**

func nextBool() -> Bool

Generates and returns a new random Boolean value.

**Required**

