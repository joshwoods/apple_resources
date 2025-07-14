

- HomeKit
- HMError
-  nilParameter 

Type Property

# nilParameter

An error indicating that nil was passed for an operation that does not accept nil.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var nilParameter: HMError.Code { get }
```

## See Also

### Detecting parameter errors

static var invalidParameter: HMError.Code

An error indicating the object is invalid for the given operation.

static var missingParameter: HMError.Code

An error indicating a missing parameter.

static var unconfiguredParameter: HMError.Code

An error indicating an unconfigured parameter.

