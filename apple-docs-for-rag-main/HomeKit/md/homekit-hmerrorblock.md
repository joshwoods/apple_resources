

- HomeKit
-  HMErrorBlock 

Type Alias

# HMErrorBlock

A completion block that provides an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias HMErrorBlock = ((any Error)?) -> Void
```

## Parameters 

`error`  

The error the block returns.

## See Also

### Errors

struct HMError

An error HomeKit returns.

let HMErrorDomain: String

A string that identifies the HomeKit error domain.

enum Code

Possible error values that can be returned from HomeKit APIs.

