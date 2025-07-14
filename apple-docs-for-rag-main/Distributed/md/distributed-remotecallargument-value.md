

- Distributed
- RemoteCallArgument
-  value 

Instance Property

# value

The value of the argument being passed to the call. As `RemoteCallArgument` is always used in conjunction with `recordArgument` and populated by the compiler, this Value will generally conform to a distributed actor system’s `SerializationRequirement`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
let value: Value
```

