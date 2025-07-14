

- Swift
-  ManagedBuffer 

Class

# ManagedBuffer

A class whose instances contain a property of type `Header` and raw storage for an array of `Element`, whose size is determined at instance creation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class ManagedBuffer where Element : ~Copyable
```

## Overview

Note that the `Element` array is suitably-aligned **raw memory**. You are expected to construct and—if necessary—destroy objects there yourself, using the APIs on `UnsafeMutablePointer`. Typical usage stores a count and capacity in `Header` and destroys any live elements in the `deinit` of a subclass.

Note

Subclasses must not have any stored properties; any storage needed should be included in `Header`.

## Topics

### Instance Properties

var capacity: Int

The actual number of elements that can be stored in this object.

var header: Header

The stored `Header` instance.

### Instance Methods

func withUnsafeMutablePointerToElements&lt;E, R>((UnsafeMutablePointer&lt;Element>) throws(E) -> R) throws(E) -> R

Call `body` with an `UnsafeMutablePointer` to the `Element` storage.

func withUnsafeMutablePointerToHeader&lt;E, R>((UnsafeMutablePointer&lt;Header>) throws(E) -> R) throws(E) -> R

Call `body` with an `UnsafeMutablePointer` to the stored `Header`.

func withUnsafeMutablePointers&lt;E, R>((UnsafeMutablePointer&lt;Header>, UnsafeMutablePointer&lt;Element>) throws(E) -> R) throws(E) -> R

Call `body` with `UnsafeMutablePointer`s to the stored `Header` and raw `Element` storage.

### Type Methods

class func create(minimumCapacity: Int, makingHeaderWith: (ManagedBuffer&lt;Header, Element>) throws -> Header) rethrows -> ManagedBuffer&lt;Header, Element>

Create a new instance of the most-derived class, calling `factory` on the partially-constructed object to generate an initial `Header`.

## See Also

### Buffer Implementation

struct ManagedBufferPointer

Contains a buffer object, and provides access to an instance of `Header` and contiguous storage for an arbitrary number of `Element` instances stored in that buffer.

