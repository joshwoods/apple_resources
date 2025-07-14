

- Swift
- Result
- Result.Publisher
-  max(by:) 

Instance Method

# max(by:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func max(by areInIncreasingOrder: (Result.Publisher.Output, Result.Publisher.Output) -> Bool) -> Result.Publisher.Output, Failure>.Publisher
```

Available when `Failure` conforms to `Error`.

