

- GameplayKit
-  GKShuffledDistribution 

Class

# GKShuffledDistribution

A generator for random numbers that are uniformly distributed across many samplings, but where short sequences of similar values are unlikely.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKShuffledDistribution
```

## Overview

The behavior of a shuffled distribution is sometimes called “fair” randomization, because true randomness in games can result in extended “lucky streaks” or “unlucky streaks” for players. To create a shuffled distribution and use it to generate random numbers, use the methods defined by its superclass GKRandomDistribution.

The GKShuffledDistribution class inherits its entire interface from its superclass—to initialize and use a shuffled distribution, use the methods listed in GKRandomDistribution. A shuffled distribution differs from its superclass in behavior only. Consider the code snippets below:

- Swift
- Objective-C

```
// Uniform distribution
let uniform = GKRandomDistribution.d6()
for _ in 1...100 { print(uniform.nextInt()) }

// Shuffled distribution
let shuffled = GKShuffledDistribution.d6()
for _ in 1...100 { print(shuffled.nextInt()) }
```

```
// Uniform distribution
GKRandomDistribution *uniform = [GKRandomDistribution d6];
for (int i = 0; i 

In this example, each distribution generates 100 random integers from a simulated six-sided die. In both cases, the distribution of results is roughly uniform—that is, the number of occurrences of any specific value is about the same as that of any other value. However, the shuffled distribution makes sure not to repeat any one value until it has used all of its possible values. In this example, if the die rolls a 1, the shuffled distribution will not generate another 1 for at least five more rolls.

Important

The randomization services provided in GameplayKit are suitable for reliably creating deterministic, pseudorandom gameplay mechanics, but are not cryptographically robust. For cryptography, obfuscation, or cipher uses, use the Security framework, described in Cryptographic Services Guide.

For more information on choosing and using randomizers in GameplayKit, read Randomization in GameplayKit Programming Guide.

## Relationships

### Inherits From

- GKRandomDistribution

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

class GKRandomDistribution

A generator for random numbers that fall within a specific range and that exhibit a specific distribution over multiple samplings.

class GKGaussianDistribution

A generator for random numbers that follow a *Gaussian distribution* (also known as a *normal distribution*) across multiple samplings.

