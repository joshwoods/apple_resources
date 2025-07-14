

- BrowserEngineKit
- RestrictedSandboxRevision
-  \

Operator

# \

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
static func  Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

This function is the only requirement of the `Comparable` protocol. The remainder of the relational operator functions are implemented by the standard library for any type that conforms to `Comparable`.

