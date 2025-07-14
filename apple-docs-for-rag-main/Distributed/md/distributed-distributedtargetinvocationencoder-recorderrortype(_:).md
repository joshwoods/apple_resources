

- Distributed
- DistributedTargetInvocationEncoder
-  recordErrorType(\_:) 

Instance Method

# recordErrorType(\_:)

Record the error type of the distributed method. This method will not be invoked if the target is not throwing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func recordErrorType(_ type: E.Type) throws where E : Error
```

**Required**

## Parameters 

`type`  

The type of error that was declared to be thrown by the invocation target. Currently this can only ever be `Error.self`.

