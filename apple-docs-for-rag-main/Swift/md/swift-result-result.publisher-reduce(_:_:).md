

- Swift
- Result
- Result.Publisher
-  reduce(\_:\_:) 

Instance Method

# reduce(\_:\_:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func reduce(
    _ initialResult: T,
    _ nextPartialResult: (T, Result.Publisher.Output) -> T
) -> Result.Publisher
```

Available when `Failure` conforms to `Error`.

