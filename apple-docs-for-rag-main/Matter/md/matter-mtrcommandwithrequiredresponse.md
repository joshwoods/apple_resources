

- Matter
-  MTRCommandWithRequiredResponse 

Class

# MTRCommandWithRequiredResponse

An object representing a single command to be invoked and the response required for the invoke to be considered successful.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRCommandWithRequiredResponse
```

## Topics

### Initializers

init(path: MTRCommandPath, commandFields: [String : Any]?, requiredResponse: [NSNumber : [String : Any]]?)

### Instance Properties

var commandFields: [String : Any]?

The command fields to pass for the command invoke. nil if this command does not have any fields. If not nil, this should be a data-value dictionary of MTRStructureValueType.

var path: MTRCommandPath

The path of the command being invoked.

var requiredResponse: [NSNumber : [String : Any]]?

The response that represents this command succeeding.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

