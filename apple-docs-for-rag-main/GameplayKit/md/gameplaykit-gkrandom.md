

- GameplayKit
-  GKRandom 

Protocol

# GKRandom

The common interface for all randomization classes in (or usable with) GameplayKit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol GKRandom
```

## Overview

Important

The randomization services provided in GameplayKit are suitable for reliably creating deterministic, pseudorandom gameplay mechanics, but are not cryptographically robust. For cryptography, obfuscation, or cipher uses, use the Security framework, described in Cryptographic Services Guide.

GameplayKit randomization classes include the GKRandomSource and GKRandomDistribution classes and their subclasses. You use those classes to generate random behavior for gameplay mechanics, and use this protocol type directly when composing random sources to create more complex randomizers.

For more information on choosing and using randomizers in GameplayKit, read Randomization in GameplayKit Programming Guide.

## Topics

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

func nextBool() -> Bool

Generates and returns a new random Boolean value.

**Required**

## Relationships

### Conforming Types

- GKARC4RandomSource
- GKGaussianDistribution
- GKLinearCongruentialRandomSource
- GKMersenneTwisterRandomSource
- GKRandomDistribution
- GKRandomSource
- GKShuffledDistribution

## See Also

### Randomization

class GKRandomSource

The superclass for all basic randomization classes in GameplayKit.

class GKARC4RandomSource

A basic random number generator implementing the ARC4 algorithm, which is suitable for most gameplay mechanics.

class GKLinearCongruentialRandomSource

A basic random number generator implementing the linear congruential generator algorithm, which is faster but less random than the default random source.

class GKMersenneTwisterRandomSource

A basic random number generator implementing the Mersenne Twister algorithm, which is more random, but slower than the default random source.

class GKRandomDistribution

A generator for random numbers that fall within a specific range and that exhibit a specific distribution over multiple samplings.

class GKGaussianDistribution

A generator for random numbers that follow a *Gaussian distribution* (also known as a *normal distribution*) across multiple samplings.

class GKShuffledDistribution

A generator for random numbers that are uniformly distributed across many samplings, but where short sequences of similar values are unlikely.

