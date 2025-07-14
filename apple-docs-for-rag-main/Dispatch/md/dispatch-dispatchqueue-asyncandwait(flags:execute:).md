

- Dispatch
- DispatchQueue
-  asyncAndWait(flags:execute:) 

Instance Method

# asyncAndWait(flags:execute:)

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
func asyncAndWait(
    flags: DispatchWorkItemFlags,
    execute work: () throws -> T
) rethrows -> T
```

