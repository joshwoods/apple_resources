

- Security
-  SSLSetMaxDatagramRecordSize(\_:\_:) Deprecated

Function

# SSLSetMaxDatagramRecordSize(\_:\_:)

Sets the maximum datagram record size allowed by the application for a given context.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLSetMaxDatagramRecordSize(
    _ dtlsContext: SSLContext,
    _ maxSize: Int
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`dtlsContext`  

The SSL context associated with the connection.

`maxSize`  

The length value.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

The size you indicate includes all Datagram Transport Layer Security (DTLS) headers.

You can specify a new value up to the maximum size of a UDP packet (which, in turn, is based on the underlying IP protocol).

