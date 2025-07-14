

- Distributed
- LocalTestingInvocationEncoder
-  recordGenericSubstitution(\_:) 

Instance Method

# recordGenericSubstitution(\_:)

The arguments must be encoded order-preserving, and once `decodeGenericSubstitutions` is called, the substitutions must be returned in the same order in which they were recorded.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func recordGenericSubstitution(_ type: T.Type) throws
```

## Parameters 

`type`  

A generic substitution type to be recorded for this invocation.

