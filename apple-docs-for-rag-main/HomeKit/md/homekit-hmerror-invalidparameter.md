

- HomeKit
- HMError
-  invalidParameter 

Type Property

# invalidParameter

An error indicating the object is invalid for the given operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var invalidParameter: HMError.Code { get }
```

## Discussion

For example, the home object issues an error when attempting to add a room that exists in another home.

## See Also

### Detecting parameter errors

static var missingParameter: HMError.Code

An error indicating a missing parameter.

static var nilParameter: HMError.Code

An error indicating that nil was passed for an operation that does not accept nil.

static var unconfiguredParameter: HMError.Code

An error indicating an unconfigured parameter.

