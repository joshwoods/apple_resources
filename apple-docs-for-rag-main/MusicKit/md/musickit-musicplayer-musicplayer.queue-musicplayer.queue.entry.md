

- MusicKit
- MusicPlayer
- MusicPlayer.Queue
-  MusicPlayer.Queue.Entry 

Structure

# MusicPlayer.Queue.Entry

An entry for the playback queue of the music player.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
struct Entry
```

## Topics

### Operators

static func == (MusicPlayer.Queue.Entry, MusicPlayer.Queue.Entry) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(any PlayableMusicItem, startTime: TimeInterval?, endTime: TimeInterval?)

Creates an entry of the playback queue with a playable music item, and optional start and end times.

### Instance Properties

var artwork: Artwork?

The artwork of this entry of the playback queue.

var description: String

A textual representation of this instance.

var endTime: TimeInterval?

An optional end time for this entry of the playback queue.

var hashValue: Int

The hash value.

let id: String

The unique identifier of this entry of the playback queue.

var isTransient: Bool

A Boolean value that indicates whether this entry of the playback queue has a transient music item.

var item: MusicPlayer.Queue.Entry.Item?

A music item that corresponds to this entry of the playback queue, such as a song or a music video.

var startTime: TimeInterval?

An optional start time for this entry of the playback queue.

var subtitle: String?

The subtitle of this entry of the playback queue.

var title: String

The title of this entry of the playback queue.

var transientItem: (any PlayableMusicItem)?

A music item that corresponds to a recently inserted entry in the playback queue that has underlying items the music player still needs to resolve.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Enumerations

enum Item

An item that corresponds to an entry in the playback queue.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Identifiable

