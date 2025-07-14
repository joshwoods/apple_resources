

- GameplayKit
- GKARC4RandomSource
-  dropValues(\_:) 

Instance Method

# dropValues(\_:)

Skips the specified number of values in the random sequence.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func dropValues(_ count: Int)
```

## Parameters 

`count`  

The number of values to skip ahead in the random source’s sequence.

## Discussion

Because the ARC4 random number generation algorithm can result in sequences with repeating initial values, examining the first 768 values in the sequence can reveal the random source’s seed and thus predict later values in the sequence. To obfuscate gameplay mechanics based on this generator, call this method with a `count` parameter of `768` or greater.

