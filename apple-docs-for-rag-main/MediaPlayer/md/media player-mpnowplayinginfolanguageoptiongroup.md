

- Media Player
-  MPNowPlayingInfoLanguageOptionGroup 

Class

# MPNowPlayingInfoLanguageOptionGroup

A grouped set of language options where only a single language option can be active at a time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
class MPNowPlayingInfoLanguageOptionGroup
```

## Overview

The `MPNowPlayingInfoLanguageOptionGroup` and MPNowPlayingInfoLanguageOption classes provide interfaces for setting information about language options, for example, audio and subtitles, in the Now Playing information area.

## Topics

### Creating a new language option group

init(languageOptions: [MPNowPlayingInfoLanguageOption], defaultLanguageOption: MPNowPlayingInfoLanguageOption?, allowEmptySelection: Bool)

Creates a new language option group with the supplied language options.

### Retrieving language option group information

var allowEmptySelection: Bool

A Boolean that indicates whether the system requires a selection for the language option group.

var defaultLanguageOption: MPNowPlayingInfoLanguageOption?

The default language option for the group.

var languageOptions: [MPNowPlayingInfoLanguageOption]

The available language options for the group.

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

### Now Playing information

Becoming a now playable app

Ensure your app is eligible to become the Now Playing app by adopting best practices for providing Now Playing info and registering for remote command center actions.

class MPNowPlayingSession

An object that manages Now Playing information and remote commands for multiple players.

class MPNowPlayingInfoCenter

An object for setting the Now Playing information for media that your app plays.

class MPNowPlayingInfoLanguageOption

A set of interfaces for setting the language option for the Now Playing item.

Language option characteristic constants

The constants for defining language characteristics.

