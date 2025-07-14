

- Security
-  SSLGetDatagramWriteSize(\_:\_:) Deprecated

Function

# SSLGetDatagramWriteSize(\_:\_:)

Provides the largest packet that the OS guarantees it can send without fragmentation.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLGetDatagramWriteSize(
    _ dtlsContext: SSLContext,
    _ bufSize: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`dtlsContext`  

The SSL context associated with the connection.

`bufSize`  

The address of a `size_t` integer for storing the length.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

Although any packet below this threshold size will not be fragmented by the OS when sent using SSLWrite(_:_:_:_:), this function provides no guarantees about whether the packet will be fragmented by routers en route. This size value is equal to the maximum Datagram Record size (set by calling SSLSetMaxDatagramRecordSize(_:_:)) minus the DTLS Record header size.

