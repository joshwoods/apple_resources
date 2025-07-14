

- Swift
- Result
- Result.Publisher
-  tryContains(where:) 

Instance Method

# tryContains(where:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryContains(where predicate: (Result.Publisher.Output) throws -> Bool) -> Result.Publisher
```

Available when `Failure` conforms to `Error`.

