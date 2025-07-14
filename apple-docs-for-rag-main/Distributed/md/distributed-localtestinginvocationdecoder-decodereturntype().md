

- Distributed
- LocalTestingInvocationDecoder
-  decodeReturnType() 

Instance Method

# decodeReturnType()

Attempt to decode the known return type of the distributed invocation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
final func decodeReturnType() throws -> (any Any.Type)?
```

## Discussion

It is legal to implement this by returning `nil`, and then the system will take the concrete return type from the located function signature.

