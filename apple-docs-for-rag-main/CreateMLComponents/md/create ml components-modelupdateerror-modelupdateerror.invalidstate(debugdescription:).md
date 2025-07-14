

- Create ML Components
- ModelUpdateError
-  ModelUpdateError.invalidState(debugDescription:) 

Case

# ModelUpdateError.invalidState(debugDescription:)

An error that indicates that a default initialized transformer suitable for fitting cannot perform apply before performing an update.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case invalidState(debugDescription: String)
```

## See Also

### Analyzing the error

var errorDescription: String?

A localized message describing what error occurred.

