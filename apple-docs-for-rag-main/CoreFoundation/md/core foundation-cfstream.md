

- Core Foundation
-  CFStream 

API Collection

# CFStream

## Overview

This document describes the generic `CFStream` functions, data types, and constants. See also CFReadStream and CFWriteStream for functions and constants specific to read and write streams respectively.

Note

When you use the `CFStream` API for networking, read and write operations on sockets can block. To prevent blocking:

1.  Call CFReadStreamSetClient(_:_:_:_:) and CFWriteStreamSetClient(_:_:_:_:) to register to receive stream-related event notifications.

2.  Call CFReadStreamScheduleWithRunLoop(_:_:_:) and CFWriteStreamScheduleWithRunLoop(_:_:_:) to schedule the stream on a run loop for receiving stream-related event notifications.

3.  Call CFReadStreamOpen(_:) and CFWriteStreamOpen(_:) to open each stream.

4.  Read only after receiving a hasBytesAvailable notification. Write only after receiving a canAcceptBytes notification.

## Topics

### Creating Streams

func CFStreamCreatePairWithPeerSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a socket.

Deprecated

func CFStreamCreatePairWithSocketToHost(CFAllocator!, CFString!, UInt32, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a TCP/IP port of a particular host.

Deprecated

func CFStreamCreatePairWithSocket(CFAllocator!, CFSocketNativeHandle, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!)

Creates readable and writable streams connected to a socket.

Deprecated

func CFStreamCreateBoundPair(CFAllocator!, UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>!, CFIndex)

Creates a bound pair of read and write streams.

func CFStreamCreatePairWithSocketToCFHost(_ alloc: CFAllocator?, _ host: CFHost, _ port: Int32, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>?, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>?)

Creates readable and writable streams connected to a given \`CFHost\` object.

Deprecated

func CFStreamCreatePairWithSocketToNetService(_ alloc: CFAllocator?, _ service: CFNetService, _ readStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFReadStream>?>?, _ writeStream: UnsafeMutablePointer&lt;Unmanaged&lt;CFWriteStream>?>?)

Creates a pair of streams for a CFNetService.

Deprecated

### Obtaining Errors

func CFSocketStreamSOCKSGetError(_ error: UnsafePointer&lt;CFStreamError>) -> Int32

This function gets error codes in the \`kCFStreamErrorDomainSOCKS\` domain from the \`CFStreamError\` returned by a stream operation.

func CFSocketStreamSOCKSGetErrorSubdomain(_ error: UnsafePointer&lt;CFStreamError>) -> Int32

Gets the error subdomain associated with errors in the \`kCFStreamErrorDomainSOCKS\` domain from the \`CFStreamError\` returned by a stream operation.

### Setting the Security Protocol

func CFReadStreamSetProperty(CFReadStream!, CFStreamPropertyKey!, CFTypeRef!) -> Bool

Sets the value of a property for a stream.

func CFWriteStreamSetProperty(CFWriteStream!, CFStreamPropertyKey!, CFTypeRef!) -> Bool

Sets the value of a property for a stream.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

### Data Types

struct CFStreamError

The structure returned by CFReadStreamGetError(_:) and CFWriteStreamGetError(_:).

struct CFStreamClientContext

A structure that contains program-defined data and callbacks with which you can configure a stream’s client behavior.

### Constants

enum CFStreamStatus

Constants that describe the status of a stream.

enum CFStreamErrorDomain

Defines constants for values returned in the domain field of the `CFStreamError` structure.

CFStream Error Domain Constants (CFHost)

Defines constants for values returned in the domain field of the `CFStreamError` structure.

Error Subdomains

Subdomains used to determine how to interpret an error in the `kCFStreamErrorDomainSOCKS` domain.

Secure Sockets (SOCKS) Errors

Error codes returned by the \`kCFStreamErrorDomainSOCKS\` error domain.

struct CFStreamEventType

Defines constants for stream-related events.

Stream Properties

Stream property names that can be set or copied.

CFStream Property SSL Settings Constants

Constants for use in a `CFDictionary` object that is the value of the `kCFStreamPropertySSLSettings` stream property key.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

Stream Service Types

String constants that specify the service type of a stream.

## See Also

### Related Documentation

Getting Started with Networking, Internet, and Web

CFNetwork Programming Guide

### Reference

Core Foundation Structures

Core Foundation Enumerations

Core Foundation Constants

Core Foundation Functions

Core Foundation Data Types

Core Foundation Macros

