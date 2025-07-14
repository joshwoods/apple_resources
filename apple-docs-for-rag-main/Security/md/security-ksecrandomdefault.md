

- Security
-  kSecRandomDefault 

Global Variable

# kSecRandomDefault

An alias for the default random number generator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecRandomDefault: SecRandomRef
```

## Discussion

When passed to the SecRandomCopyBytes(_:_:_:) function as the random number generator reference, this constant indicates that the default number generator should be used.

This constant is a synonym for `NULL`.

