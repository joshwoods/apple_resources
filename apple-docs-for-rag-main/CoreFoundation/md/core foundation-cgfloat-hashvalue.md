

- Core Foundation
- CGFloat
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOSwatchOS 1.0+

``` source
var hashValue: Int { get }
```

## Discussion

**Axiom:** `x == y` implies `x.hashValue == y.hashValue`.

Note

The hash value is not guaranteed to be stable across different invocations of the same program. Do not persist the hash value across program runs.

