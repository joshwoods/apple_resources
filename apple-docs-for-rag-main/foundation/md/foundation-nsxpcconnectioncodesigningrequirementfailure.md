

- Foundation
-  NSXPCConnectionCodeSigningRequirementFailure 

Global Variable

# NSXPCConnectionCodeSigningRequirementFailure

A code-signing requirement check failed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var NSXPCConnectionCodeSigningRequirementFailure: Int { get }
```

## Discussion

This error represents a failure to meet the requirement set by a call to NSXPCConnection‘s setCodeSigningRequirement(_:) method, or NSXPCConnectionListener’s setConnectionCodeSigningRequirement(_:) method.

## See Also

### Error codes

var NSXPCConnectionInterrupted: Int

The XPC connection was interrupted.

var NSXPCConnectionInvalid: Int

The XPC connection was invalid.

var NSXPCConnectionReplyInvalid: Int

The XPC connection reply was invalid.

var NSXPCConnectionErrorMinimum: Int

The lower bounds of XPC connection error code values.

var NSXPCConnectionErrorMaximum: Int

The upper bounds of XPC connection error code values.

