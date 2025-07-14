

- Metal
-  MTLIOCommandBuffer 

Protocol

# MTLIOCommandBuffer

A command buffer that contains input/output commands that work with files in the file systems and Metal resources.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLIOCommandBuffer : NSObjectProtocol
```

## Overview

Add commands an input/output command buffer to load assets from the file system directly into Metal resources. Your app can then use those resources with other commands it submits to MTLCommandQueue.

## Topics

### Loading Assets

func load(any MTLBuffer, offset: Int, size: Int, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into a GPU buffer.

**Required**

func load(any MTLTexture, slice: Int, level: Int, size: MTLSize, sourceBytesPerRow: Int, sourceBytesPerImage: Int, destinationOrigin: MTLOrigin, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into a GPU texture.

**Required**

func loadBytes(UnsafeMutableRawPointer, size: Int, sourceHandle: any MTLIOFileHandle, sourceHandleOffset: Int)

Encodes a command that loads data from a file handle into CPU-accessible memory buffer.

**Required**

### Adding a Barrier

func addBarrier()

Encodes a barrier into the command buffer.

**Required**

### Synchronizing a Command Buffer

func signalEvent(any MTLSharedEvent, value: UInt64)

Encodes a command that signals a shared event to other parts of your app.

**Required**

func waitForEvent(any MTLSharedEvent, value: UInt64)

Encodes a command that pauses the command buffer’s execution until another part of your app signals a shared event.

**Required**

### Adding Final Commands

func copyStatus(buffer: any MTLBuffer, offset: Int)

Encodes a command that writes the input/output command buffer’s status to a buffer.

**Required**

func addCompletedHandler(MTLIOCommandBufferHandler)

Adds a closure that Metal calls immediately after the GPU finishes executing the commands in the input/output command buffer.

**Required**

### Submitting a Command Buffer

func commit()

Submits the command buffer to the queue for execution on the GPU.

**Required**

func enqueue()

Reserves a place for the input/output command buffer in the input/output command queue without committing the command buffer.

**Required**

### Canceling a Command Buffer

func tryCancel()

Submits a request to abandon a command buffer the queue is currently running.

**Required**

### Waiting for a Command Buffer

func waitUntilCompleted()

Blocks the current thread until the GPU finishes executing the input/output command buffer and all of its completion handlers.

**Required**

### Checking the State of a Command Buffer

var status: MTLIOStatus

Represents the state of the input/output command buffer.

**Required**

var error: (any Error)?

Stores the details of an error when the GPU experienced a problem with the input/output command buffer.

**Required**

### Debugging a Command Buffer

var label: String?

An optional name for the input/output command buffer.

**Required**

func pushDebugGroup(String)

Sets the current name for this input/output command encoder by adding it to the top of the debug name stack.

**Required**

func popDebugGroup()

Restores the previous name for this input/output command encoder by removing the top item of the debug name stack.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### I/O Command Buffers

protocol MTLIOFileHandle

Represents a raw or compressed file, such as a resource asset file in your app’s bundle.

typealias MTLIOCommandBufferHandler

A convenience type that defines the signature of an input/output command buffer’s completion handler.

enum MTLIOStatus

Represents the state of an input/output command buffer.

enum Code

The error codes for creating an input/output file handle.

let MTLIOErrorDomain: String

The domain for input/output command queue errors.

