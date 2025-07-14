

- ShazamKit
-  SHSessionDelegate 

Protocol

# SHSessionDelegate

Methods that the session calls with the result of a match request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol SHSessionDelegate : NSObjectProtocol
```

## Topics

### Handling matches

func session(SHSession, didFind: SHMatch)

Tells the delegate that the query signature matches an item in the catalog.

func session(SHSession, didNotFindMatchFor: SHSignature, error: (any Error)?)

Tells the delegate that the query signature doesn’t match an item in the catalog, or that there’s an error.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Match audio

class SHSession

An object that matches a specific audio recording when a segment of that recording is part of captured sound in the Shazam catalog or your custom catalog.

class SHManagedSession

An object that records and matches a recording with captured sound in the Shazam catalog or your custom catalog.

class SHMatch

An object that represents the catalog media items that match a query.

class SHMatchedMediaItem

An object that represents the metadata for a matched reference signature.

class SHMediaItem

An object that represents the metadata for a reference signature.

