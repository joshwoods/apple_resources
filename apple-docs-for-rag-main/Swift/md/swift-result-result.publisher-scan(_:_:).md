

- Swift
- Result
- Result.Publisher
-  scan(\_:\_:) 

Instance Method

# scan(\_:\_:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scan(
    _ initialResult: T,
    _ nextPartialResult: (T, Result.Publisher.Output) -> T
) -> Result.Publisher
```

Available when `Failure` conforms to `Error`.

