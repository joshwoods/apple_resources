

- Swift
- Result
- Result.Publisher
-  tryMap(\_:) 

Instance Method

# tryMap(\_:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryMap(_ transform: (Result.Publisher.Output) throws -> T) -> Result.Publisher
```

Available when `Failure` conforms to `Error`.

