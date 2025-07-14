

- GSS
-  kGSSICAppleSourceAppAuditToken 

Global Variable

# kGSSICAppleSourceAppAuditToken

The audit token of the app’s process.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var kGSSICAppleSourceAppAuditToken: String { get }
```

## Discussion

The value is an `audit_token_t` value wrapped in a `CFDataRef`.

## See Also

### Apple Source App Keys

var kGSSICAppleSourceAppPID: String

A number that indicates the process ID of the app.

var kGSSICAppleSourceAppSigningIdentity: String

The bundle signing identity of the app.

