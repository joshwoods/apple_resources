

- ShazamKit
-  SHSession 

Class

# SHSession

An object that matches a specific audio recording when a segment of that recording is part of captured sound in the Shazam catalog or your custom catalog.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHSession
```

## Mentioned in 

Matching audio using the built-in microphone

## Overview

Prepare to make matches by:

- Creating a session for the catalog that contains the reference signatures

- Adding your delegate that receives the match results

Search for a match in one of two ways:

- Generate a signature for the captured audio and call match(_:)

- Call matchStreamingBuffer(_:at:) with a streaming audio buffer, and ShazamKit generates the signature for you

Searching the catalog is asynchronous. The session calls your delegate methods with the result.

Matching songs in Shazam music requires enabling your app to access the catalog. For more information on enabling your app, see Enable ShazamKit for an App ID.

The code below shows searching for a match in the Shazam catalog using an existing audio buffer:

```
// Set up the session.
let session = SHSession()
session.delegate = self

// Create a signature from the captured audio buffer.
let signatureGenerator = SHSignatureGenerator()
try signatureGenerator.append(buffer, at: audioTime)
let signature = signatureGenerator.signature()

// Check for a match.
session.match(signature)

// The delegate method that the session calls when matching a reference item.
func session(_ session: SHSession, didFind match: SHMatch) {
    // Do something with the matched results.
}

// The delegate method that the session calls when there is no match.
 func session(_ session: SHSession, didNotFindMatchFor signature: SHSignature, error: Error?) {
    // No match found.
}
```

## Topics

### Creating a session object

init()

Creates a new session object for matching songs in the Shazam Music catalog.

init(catalog: SHCatalog)

Creates a new session object for matching audio in a custom catalog.

### Making a match

func match(SHSignature)

Searches for the query signature in the reference signatures that the session catalog contains.

func matchStreamingBuffer(AVAudioPCMBuffer, at: AVAudioTime?)

Converts the audio in the buffer to a signature, and searches the reference signatures in the session catalog.

Matching audio using the built-in microphone

Use the audio stream from the microphone as the source for a ShazamKit session.

### Reading the session properties

var delegate: (any SHSessionDelegate)?

The object that the session calls with the result of a match request.

var catalog: SHCatalog

The catalog object containing the reference signatures and their associated metadata that the session uses to perform matches.

var results: SHSession.Results

The results as an asynchronous sequence of matches.

struct Results

An asynchronous sequence that emits updates from a session object query.

### Returning queries

func result(from: SHSignature) async -> SHSession.Result

Performs an asynchronous match with a signature you specify.

enum Result

Identifies the result from an asynchronous sequence result.

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

## See Also

### Match audio

class SHManagedSession

An object that records and matches a recording with captured sound in the Shazam catalog or your custom catalog.

protocol SHSessionDelegate

Methods that the session calls with the result of a match request.

class SHMatch

An object that represents the catalog media items that match a query.

class SHMatchedMediaItem

An object that represents the metadata for a matched reference signature.

class SHMediaItem

An object that represents the metadata for a reference signature.

