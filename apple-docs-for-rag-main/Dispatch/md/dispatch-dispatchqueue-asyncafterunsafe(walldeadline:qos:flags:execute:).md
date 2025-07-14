

- Dispatch
- DispatchQueue
-  asyncAfterUnsafe(wallDeadline:qos:flags:execute:) 

Instance Method

# asyncAfterUnsafe(wallDeadline:qos:flags:execute:)

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func asyncAfterUnsafe(
    wallDeadline: DispatchWallTime,
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    execute work: @escaping () -> Void
)
```

