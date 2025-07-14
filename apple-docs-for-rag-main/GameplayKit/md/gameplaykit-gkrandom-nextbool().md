

- GameplayKit
- GKRandom
-  nextBool() 

Instance Method

# nextBool()

Generates and returns a new random Boolean value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nextBool() -> Bool
```

**Required**

## Return Value

A random Boolean value.

## Discussion

Typically, custom classes implementing this protocol should implement the nextBool() method based on the value returned by the nextInt(upperBound:) method. Alternative implementations are possible, but may lead to less uniform results.

## See Also

### Generating Random Numbers

func nextInt() -> Int

Generates and returns a new random integer.

**Required**

func nextInt(upperBound: Int) -> Int

Generates and returns a new random integer less than the specified limit.

**Required**

func nextUniform() -> Float

Generates and returns a new random floating-point value.

**Required**

