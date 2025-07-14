

- Swift
- Result
- Result.Publisher
-  setFailureType(to:) 

Instance Method

# setFailureType(to:)

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func setFailureType(to failureType: E.Type) -> Result.Publisher.Output, E>.Publisher where E : Error
```

Available when `Failure` is `Never`.

