

- AppKit
- Deprecated Symbols
- NSOpenGLPixelFormat
-  OpenGL Profiles 

API Collection

# OpenGL Profiles

Constants that specify the functionality provided by the renderer.

## Overview

An OpenGL Profile is requested as part of the pixel format attributes string. When a context is created for a profile, the context must at least implement the requested version of the OpenGL specification. The context may implement a different version of the OpenGL specification as long as the version it implements is compatible with the requested version.

## Topics

### Constants

var NSOpenGLProfileVersionLegacy: Int

The requested profile is a legacy (pre-OpenGL 3.0) profile.

Deprecated

var NSOpenGLProfileVersion3_2Core: Int

The requested profile must implement the OpenGL 3.2 core functionality.

Deprecated

var NSOpenGLProfileVersion4_1Core: IntDeprecated

## See Also

### Constants

typealias NSOpenGLPixelFormatAttribute

Pixel format attributes for OpenGL.

Deprecated

OpenGL Pixel Format Attributes

Pixel format attributes for OpenGL.

