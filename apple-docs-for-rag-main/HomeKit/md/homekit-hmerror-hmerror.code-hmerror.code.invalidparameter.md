

- HomeKit
- HMError
- HMError.Code
-  HMError.Code.invalidParameter 

Case

# HMError.Code.invalidParameter

An error indicating the object is invalid for the given operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
case invalidParameter
```

## Discussion

For example, the home object issues an error when attempting to add a room that exists in another home.

## See Also

### Parameter errors

case missingParameter

An error indicating a missing parameter.

case nilParameter

An error indicating that `nil` was passed for an operation that does not accept `nil`.

case unconfiguredParameter

An error indicating an unconfigured parameter.

