

- AppKit
-  NSSound 

Class

# NSSound

A simple interface for loading and playing audio files.

macOS

``` source
class NSSound
```

## Overview

You create a sound object with an audio file or data, which can be in any format that Core Audio supports. Customize the sound by configuring its properties, such as setting its playback volume and looping behavior. Call the sound’s play() method to begin playback. The system executes this call asynchronously so that it doesn’t interrupt the functioning of your app.

If you want to play the system beep sound, use the beep() (Swift) or NSBeep (Objective-C) function.

## Topics

### Detecting When a Sound Finishes Playing

var delegate: (any NSSoundDelegate)?

The sound’s delegate.

protocol NSSoundDelegate

A set of optional methods implemented by delegates of NSSound objects.

### Creating Sounds

class func canInit(with: NSPasteboard) -> Bool

Indicates whether the receiver can create an instance of itself from the data in a pasteboard.

init?(contentsOfFile: String, byReference: Bool)

Initializes the receiver with the audio data located at a given filepath.

init?(contentsOf: URL, byReference: Bool)

Initializes the receiver with the audio data located at a given URL.

init?(data: Data)

Initializes the receiver with a given audio data.

init?(pasteboard: NSPasteboard)

Initializes the receiver with data from a pasteboard. The pasteboard should contain a type returned by NSSound. `NSSound` expects the data to have a proper magic number, sound header, and data for the formats it supports.

### Configuring Sounds

var name: NSSound.Name?

The name assigned to the sound.

typealias Name

func setName(NSSound.Name?) -> Bool

var volume: Float

The volume of the sound.

var currentTime: TimeInterval

The sound’s playback progress, in seconds.

var loops: Bool

A Boolean that indicates whether the sound restarts playback when it reaches the end of its content.

var playbackDeviceIdentifier: NSSound.PlaybackDeviceIdentifier?

Identifies the sound’s output device

typealias PlaybackDeviceIdentifier

### Getting Sound Information

class var soundUnfilteredTypes: [String]

Provides the file types the `NSSound` class understands.

init?(named: NSSound.Name)

Returns the `NSSound` instance associated with a given name.

var duration: TimeInterval

The duration of the sound, in seconds.

### Playing Sounds

static func beep()

Plays the system beep.

var isPlaying: Bool

A Boolean that indicates whether the sound is playing its audio data.

func pause() -> Bool

Pauses audio playback.

func play() -> Bool

Initiates audio playback.

func resume() -> Bool

Resumes audio playback.

func stop() -> Bool

Concludes audio playback.

### Writing Sounds

func write(to: NSPasteboard)

Writes the receiver’s data to a pasteboard.

### Constants

NSPasteboard Type for Sound Data

The `NSSound` class defines this common pasteboard data type.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSPasteboardReading
- NSPasteboardWriting
- NSSecureCoding
- Transferable

