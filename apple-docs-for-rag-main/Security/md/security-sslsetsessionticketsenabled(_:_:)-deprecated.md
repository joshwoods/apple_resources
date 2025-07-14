

- Security
-  SSLSetSessionTicketsEnabled(\_:\_:) Deprecated

Function

# SSLSetSessionTicketsEnabled(\_:\_:)

Enables or disables session ticket resumption.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15Deprecated

``` source
func SSLSetSessionTicketsEnabled(
    _ context: SSLContext,
    _ enabled: Bool
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

A session context.

`enabled`  

A Boolean set to true to enable session ticket resumption, or false to disable it.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

By default, session tickets are disabled.

