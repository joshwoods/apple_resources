

- OpenGL ES
-  EAGLContext Deprecated

Class

# EAGLContext

An EAGLContext object manages an OpenGL ES *rendering context*—the state information, commands, and resources needed to draw using OpenGL ES. To execute OpenGL ES commands, you need a current rendering context.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0DeprecatedMac Catalyst 2.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
class EAGLContext
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

Drawing resources, such as textures and renderbuffers, are managed for the EAGLContext object by an EAGLSharegroup object associated with the context. When you initialize a new EAGLContext object, you can choose to have it create a new sharegroup, or you can use one obtained from a previously created context.

Before drawing to a context, you must bind a complete framebuffer object to the context. For more information on configuring rendering contexts, see OpenGL ES Programming Guide.

## Topics

### Creating Contexts

convenience init?(api: EAGLRenderingAPI)

Initializes and returns a newly allocated rendering context with the specified version of the OpenGL ES rendering API.

init?(api: EAGLRenderingAPI, sharegroup: EAGLSharegroup)

Initializes and returns a newly allocated rendering context with the specified version of OpenGL ES rendering API and the specified sharegroup.

### Setting the Current Context

class func setCurrent(EAGLContext?) -> Bool

Makes the specified context the current rendering context for the calling thread.

### Attaching Storage to a Renderbuffer

func renderbufferStorage(Int, from: (any EAGLDrawable)?) -> Bool

Binds a drawable object’s storage to an OpenGL ES renderbuffer object.

### Displaying a Renderbuffer

func presentRenderbuffer(Int) -> Bool

Displays a renderbuffer’s contents on screen.

### Getting Context Information

var api: EAGLRenderingAPI

The OpenGL ES rendering API version supported by the context. (read-only)

var sharegroup: EAGLSharegroup

The context’s sharegroup object. (read-only)

var debugLabel: String?

A label describing the context for use in debugging.

class func current() -> EAGLContext?

Returns the current rendering context for the calling thread.

### Enabling OpenGL ES Multithreading

var isMultiThreaded: Bool

A Boolean value that determines whether OpenGL ES defers work to another thread.

### Constants

enum EAGLRenderingAPI

Versions of OpenGL ES that a rendering context provides.

### Instance Methods

func presentRenderbuffer(Int, afterMinimumDuration: CFTimeInterval) -> Bool

func presentRenderbuffer(Int, atTime: CFTimeInterval) -> Bool

func texImageIOSurface(IOSurfaceRef, target: Int, internalFormat: Int, width: UInt32, height: UInt32, format: Int, type: Int, plane: UInt32) -> Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

