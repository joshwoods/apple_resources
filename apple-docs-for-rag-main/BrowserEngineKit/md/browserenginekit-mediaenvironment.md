

- BrowserEngineKit
-  MediaEnvironment 

Structure

# MediaEnvironment

An object that identifies a media playback or streaming environment.

iOS 17.4+iPadOS 17.4+

``` source
struct MediaEnvironment
```

## Overview

To stream media in your browser app, create an instance of `MediaEnvironment` in the app. In the app, call activate() before you begin any media playback or capture, including using the AVCaptureSession that you get by calling makeCaptureSession(). When you are done with the media environment, call suspend().

If you capture media input or prepare streaming content in your browser’s rendering extension, call activate() before calling grantCapability(_:) to grant a media playback and capture capability, which you create with ProcessCapability.mediaPlaybackAndCapture(environment:). Call createXPCRepresentation() and use XPC to send the media environment to the rendering extension. Additionally, grant the same capability to the web content extension for the page that’s playing or capturing media, by calling grantCapability(_:).

## Topics

### Creating a media environment

init(webPage: URL)

Creates a new media environment identified by the URL.

init(xpcRepresentation: xpc_object_t) throws

Creates a media environment from an XPC representation.

### Sending media environments over XPC connections

func createXPCRepresentation() -> xpc_object_t

Creates an encoded representation of the media environment, suitable for sending over an XPC connection.

### Capturing media streams

func activate() throws

Activates the media environment.

func makeCaptureSession() throws -> AVCaptureSession

Creates a new capture session in this media environment or throws an error if it can not be created.

func suspend() throws

Suspends the media environment.

## See Also

### Extension capabilities

enum ProcessCapability

An enumeration that identifies capabilities that a browser app can grant to its extension processes.

