

- GameplayKit
- GKRandom
-  nextUniform() 

Instance Method

# nextUniform()

Generates and returns a new random floating-point value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextUniform() -> Float
```

**Required**

## Return Value

A random floating-point value in the range `[0.0, 1.0]`.

## Discussion

The distribution of multiple samplings is uniform within the range `[0.0, 1.0]`; that is, the probability of this method returning any one value is approximately equal to that of returning any other value.

Typically, custom classes implementing this protocol should implement the nextUniform() method based on the value returned by the nextInt(upperBound:) method. Alternative implementations are possible, but may lead to less uniform results.

## See Also

### Generating Random Numbers

func nextInt() -> Int

Generates and returns a new random integer.

**Required**

func nextInt(upperBound: Int) -> Int

Generates and returns a new random integer less than the specified limit.

**Required**

func nextBool() -> Bool

Generates and returns a new random Boolean value.

**Required**

