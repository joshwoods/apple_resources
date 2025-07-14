

- MusicKit
-  MusicSubscription 

Structure

# MusicSubscription

A representation of the current state of the user’s subscription to Apple Music.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicSubscription
```

## Topics

### Structures

struct Updates

An asynchronous sequence to use for observing updates to the current state of the user’s subscription to Apple Music.

### Operators

static func == (MusicSubscription, MusicSubscription) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let canBecomeSubscriber: Bool

A capability that allows your app to present subscription offers for Apple Music.

let canPlayCatalogContent: Bool

A capability that allows your app to play subscription content using a music player.

var description: String

A textual representation of this instance.

let hasCloudLibraryEnabled: Bool

A capability that allows your app to perform modifications to the user’s iCloud Music Library.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var current: MusicSubscription

The current state of the user’s subscription to Apple Music.

static var subscriptionUpdates: MusicSubscription.Updates

An asynchronous sequence to use for observing updates to the current state of the user’s subscription to Apple Music.

### Enumerations

enum Error

An error that MusicKit can throw upon requesting the current music subscription of the user.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Apple Music Subscription

struct MusicSubscriptionOffer

A type for grouping other types for showing subscription offers for Apple Music.

