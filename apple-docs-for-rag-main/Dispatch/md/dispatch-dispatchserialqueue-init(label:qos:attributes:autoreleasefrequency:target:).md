

- Dispatch
- DispatchSerialQueue
-  init(label:qos:attributes:autoreleaseFrequency:target:) 

Initializer

# init(label:qos:attributes:autoreleaseFrequency:target:)

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
convenience init(
    label: String,
    qos: DispatchQoS = .unspecified,
    attributes: DispatchSerialQueue.Attributes = [],
    autoreleaseFrequency: DispatchQueue.AutoreleaseFrequency = .workItem,
    target: DispatchQueue? = nil
)
```

