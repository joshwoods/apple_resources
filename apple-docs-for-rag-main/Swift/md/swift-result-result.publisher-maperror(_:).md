

- Swift
- Result
- Result.Publisher
-  mapError(\_:) 

Instance Method

# mapError(\_:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func mapError(_ transform: (Failure) -> E) -> Result.Publisher.Output, E>.Publisher where E : Error
```

Available when `Failure` conforms to `Error`.

