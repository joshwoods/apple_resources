

- Distributed
- LocalTestingInvocationDecoder
-  decodeGenericSubstitutions() 

Instance Method

# decodeGenericSubstitutions()

Decode all generic substitutions that were recorded for this invocation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
final func decodeGenericSubstitutions() throws -> [any Any.Type]
```

## Return Value

Array of all generic substitutions necessary to execute this invocation target.

## Discussion

The values retrieved from here must be in the same order as they were recorded by recordGenericSubstitution(_:).

Throws

If decoding substitutions fails.

