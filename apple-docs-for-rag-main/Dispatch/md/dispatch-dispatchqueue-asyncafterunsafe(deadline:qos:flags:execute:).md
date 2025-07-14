

- Dispatch
- DispatchQueue
-  asyncAfterUnsafe(deadline:qos:flags:execute:) 

Instance Method

# asyncAfterUnsafe(deadline:qos:flags:execute:)

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func asyncAfterUnsafe(
    deadline: DispatchTime,
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    execute work: @escaping () -> Void
)
```

