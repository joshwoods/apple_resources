

- Dispatch
- DispatchQueue
- DispatchQueue.SchedulerOptions
-  init(qos:flags:group:) 

Initializer

# init(qos:flags:group:)

Creates a dispatch queue scheduler options instance with the given options.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    group: DispatchGroup? = nil
)
```

