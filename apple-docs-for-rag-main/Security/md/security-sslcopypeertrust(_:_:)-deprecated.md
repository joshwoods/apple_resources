

- Security
-  SSLCopyPeerTrust(\_:\_:) Deprecated

Function

# SSLCopyPeerTrust(\_:\_:)

Retrieves a trust management object for the certificate used by a session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.15Deprecated

``` source
func SSLCopyPeerTrust(
    _ context: SSLContext,
    _ trust: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`trust`  

On return, a trust management object you can use to evaluate trust for the certificate used by the session. A trust management object includes the certificate to be verified plus the policy or policies to be used in evaluating trust. See Certificate, Key, and Trust Services for functions to create and evaluate trust management objects. You must call the `CFRelease` function for this object when you are finished with it.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

This function is valid any time after a handshake attempt.

