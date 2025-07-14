

- GameplayKit
-  GKRandomDistribution 

Class

# GKRandomDistribution

A generator for random numbers that fall within a specific range and that exhibit a specific distribution over multiple samplings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKRandomDistribution
```

## Overview

Important

The randomization services provided in GameplayKit are suitable for reliably creating deterministic, pseudorandom gameplay mechanics, but are not cryptographically robust. For cryptography, obfuscation, or cipher uses, use the Security framework, described in Cryptographic Services Guide.

You choose the algorithm that randomizes source values for a distribution by initializing it with an instance of any class that implements the GKRandom protocol, such as a basic random source (a subclass of GKRandomSource) or another random distribution. The GKRandomDistribution class itself implements a uniform distribution—for more specialized distributions use one of the subclasses GKGaussianDistribution and GKShuffledDistribution.

In a *uniform* distribution, the probability of generating any number in a specified range (between the values of the distribution’s lowestValue and highestValue properties) is approximately equal. In other words, there is no bias toward any possible outcome. To generate random numbers in this range, use the methods from the GKRandom protocol listed in Generating Random Numbers below.

For more information on choosing and using randomizers in GameplayKit, read Randomization in GameplayKit Programming Guide.

## Topics

### Creating a Random Distribution

init(randomSource: any GKRandom, lowestValue: Int, highestValue: Int)

Initializes a uniform random distribution with the specified lower and upper bounds, using the specified source randomizer.

convenience init(lowestValue: Int, highestValue: Int)

Creates a random distribution with the specified lower and upper bounds, using the Arc4 randomizer.

### Creating Specific Random Distributions

class func d6() -> Self

Creates a random distribution equivalent to a six-sided die.

class func d20() -> Self

Creates a random distribution equivalent to a twenty-sided die.

convenience init(forDieWithSideCount: Int)

Creates a random distribution equivalent to a die with the specified number of sides.

### Generating Random Numbers

func nextInt() -> Int

Generates and returns a new random integer within the bounds of the distribution.

func nextInt(upperBound: Int) -> Int

Generates and returns a new random integer within the bounds of the distribution and less than the specified limit.

func nextUniform() -> Float

Generates and returns a new random floating-point value within the characteristics of the distribution.

func nextBool() -> Bool

Generates and returns a new random Boolean value within the characteristics of the distribution.

### Working with Characteristics of a Distribution

var lowestValue: Int

The lowest value to be produced by the distribution.

var highestValue: Int

The highest value to be produced by the distribution.

var numberOfPossibleOutcomes: Int

The number of unique values the distribution can generate.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKGaussianDistribution
- GKShuffledDistribution

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKRandom
- Hashable
- NSObjectProtocol

## See Also

### Randomization

protocol GKRandom

The common interface for all randomization classes in (or usable with) GameplayKit.

class GKRandomSource

The superclass for all basic randomization classes in GameplayKit.

class GKARC4RandomSource

A basic random number generator implementing the ARC4 algorithm, which is suitable for most gameplay mechanics.

class GKLinearCongruentialRandomSource

A basic random number generator implementing the linear congruential generator algorithm, which is faster but less random than the default random source.

class GKMersenneTwisterRandomSource

A basic random number generator implementing the Mersenne Twister algorithm, which is more random, but slower than the default random source.

class GKGaussianDistribution

A generator for random numbers that follow a *Gaussian distribution* (also known as a *normal distribution*) across multiple samplings.

class GKShuffledDistribution

A generator for random numbers that are uniformly distributed across many samplings, but where short sequences of similar values are unlikely.

