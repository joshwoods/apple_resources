

- Swift
- Result
- Result.Publisher
-  tryRemoveDuplicates(by:) 

Instance Method

# tryRemoveDuplicates(by:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryRemoveDuplicates(by predicate: (Result.Publisher.Output, Result.Publisher.Output) throws -> Bool) -> Result.Publisher.Output, any Error>.Publisher
```

Available when `Failure` conforms to `Error`.

