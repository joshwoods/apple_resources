

- Security
-  SSLCreateContext(\_:\_:\_:) Deprecated

Function

# SSLCreateContext(\_:\_:\_:)

Allocates and returns a new context.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
func SSLCreateContext(
    _ alloc: CFAllocator?,
    _ protocolSide: SSLProtocolSide,
    _ connectionType: SSLConnectionType
) -> SSLContext?
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`alloc`  

The allocator to use. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`protocolSide`  

Either SSLProtocolSide.serverSide or SSLProtocolSide.clientSide.

`connectionType`  

Either SSLConnectionType.streamType or SSLConnectionType.datagramType.

## Return Value

A new context. In Objective-C, use CFRelease to release this object’s memory when you are done with it.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

