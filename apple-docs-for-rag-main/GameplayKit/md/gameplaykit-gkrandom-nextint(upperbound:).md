

- GameplayKit
- GKRandom
-  nextInt(upperBound:) 

Instance Method

# nextInt(upperBound:)

Generates and returns a new random integer less than the specified limit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextInt(upperBound: Int) -> Int
```

**Required**

## Parameters 

`upperBound`  

A limit on the values of random numbers to generate.

## Return Value

A new random integer greater than or equal to zero and less than the value of the `upperBound` parameter.

## See Also

### Generating Random Numbers

func nextInt() -> Int

Generates and returns a new random integer.

**Required**

func nextUniform() -> Float

Generates and returns a new random floating-point value.

**Required**

func nextBool() -> Bool

Generates and returns a new random Boolean value.

**Required**

