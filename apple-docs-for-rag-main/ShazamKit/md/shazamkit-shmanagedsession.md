

- ShazamKit
-  SHManagedSession 

Class

# SHManagedSession

An object that records and matches a recording with captured sound in the Shazam catalog or your custom catalog.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final class SHManagedSession
```

## Overview

This session is an alternative for SHSession if you prefer ShazamKit to manage recording.

There are two main differences between this managed session and the SHSession:

- SHManagedSession performs all recording of audio and signature generation.

- SHManagedSession won’t accept audio or Signatures that it didn’t generate.

Matching songs in Shazam requires enabling your app to access the catalog. For more information on enabling your app, see Enable ShazamKit for an App ID.

The code below shows searching for a match in the Shazam catalog using SHManagedSession:

```
```

## Topics

### Creating a managed session object

init()

Creates a new managed session object for matching songs in the Shazam Music catalog.

init(catalog: SHCatalog)

Creates a new managed session object for matching audio in a custom catalog.

### Getting the session state

var state: SHManagedSession.State

The current state of the managed session.

enum State

The state of a managed session.

### Returning queries

func result() async -> SHSession.Result

Performs an asynchronous match with a single signature.

var results: SHSession.Results

The results as an asynchronous sequence of matches.

func cancel()

Cancels the currently running match attempt.

func prepare() async

Preallocates the resources needed for a match, which increases the responsiveness of matches.

## Relationships

### Conforms To

- Copyable
- Observable
- Sendable

## See Also

### Match audio

class SHSession

An object that matches a specific audio recording when a segment of that recording is part of captured sound in the Shazam catalog or your custom catalog.

protocol SHSessionDelegate

Methods that the session calls with the result of a match request.

class SHMatch

An object that represents the catalog media items that match a query.

class SHMatchedMediaItem

An object that represents the metadata for a matched reference signature.

class SHMediaItem

An object that represents the metadata for a reference signature.

