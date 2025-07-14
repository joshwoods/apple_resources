

- Foundation
-  NSXPCCoder 

Class

# NSXPCCoder

A coder that encodes and decodes objects that your app sends over an XPC connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSXPCCoder
```

## Overview

If you want to perform custom encoding or decoding of Codable objects that your app sends over an NSXPCConnection, use isKind(of:) to determine if the coder provided to your object is a kind of NSXPCCoder.

## Topics

### Inspecting the Coder

var connection: NSXPCConnection?

The connection currently performing encoding or decoding.

var userInfo: (any NSObjectProtocol)?

An optional user information object associated with the coder.

### Encoding and Decoding

func encodeXPCObject(xpc_object_t, forKey: String)

Encodes an object to send over an XPC connection.

func decodeXPCObject(ofType: xpc_type_t, forKey: String) -> xpc_object_t?

Decodes an object and validates that its type matches the type a service provides over XPC.

## Relationships

### Inherits From

- NSCoder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### XPC Client

protocol NSXPCProxyCreating

Methods for creating new proxy objects.

class NSXPCConnection

A bidirectional communication channel between two processes.

class NSXPCInterface

An interface that may be sent to an exported object or remote object proxy.

