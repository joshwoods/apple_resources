

- Swift
- Result
- Result.Publisher
-  replaceError(with:) 

Instance Method

# replaceError(with:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func replaceError(with output: Result.Publisher.Output) -> Result.Publisher.Output, Never>.Publisher
```

Available when `Failure` conforms to `Error`.

