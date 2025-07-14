

- Dispatch
- DispatchWorkloop
-  init(label:attributes:autoreleaseFrequency:osWorkgroup:) 

Initializer

# init(label:attributes:autoreleaseFrequency:osWorkgroup:)

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
convenience init(
    label: String,
    attributes: DispatchWorkloop.Attributes = [],
    autoreleaseFrequency: DispatchQueue.AutoreleaseFrequency = .workItem,
    osWorkgroup: WorkGroup? = nil
)
```

