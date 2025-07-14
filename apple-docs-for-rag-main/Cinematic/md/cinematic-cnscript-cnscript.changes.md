

- Cinematic
- CNScript
-  CNScript.Changes 

Structure

# CNScript.Changes

An object that represents a snapshot of the changes made to a movie script, including the added user decisions and detection tracks.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
struct Changes
```

## Overview

Use as a snapshot to quickly revert to previously saved edits.

## Topics

### Initializers

init?(dataRepresentation: Data)

Creates a previously saved data representation.

### Instance Properties

var addedDetectionTracks: [CNDetectionTrack]

All detection tracks added since recording the movie.

var dataRepresentation: Data

Persistent data representation of changes for later restoration.

var fNumber: Float

The f/number to apply to the entire movie.

var userDecisions: [CNDecision]

All active user decisions, including those made at recording time, unless removed.

