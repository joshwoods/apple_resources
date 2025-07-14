

- Media Player
-  MPNowPlayingInfoLanguageOption 

Class

# MPNowPlayingInfoLanguageOption

A set of interfaces for setting the language option for the Now Playing item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
class MPNowPlayingInfoLanguageOption
```

## Overview

The MPNowPlayingInfoLanguageOption and MPNowPlayingInfoLanguageOptionGroup classes provide interfaces for setting information about language options, for example, audio and subtitles, in the Now Playing information area.

## Topics

### Creating a new language option

init(type: MPNowPlayingInfoLanguageOptionType, languageTag: String, characteristics: [String]?, displayName: String, identifier: String)

Creates a single language option.

### Retrieving language option properties

var displayName: String?

The display name for a language option.

var identifier: String?

The unique identifier for the language option.

var languageOptionCharacteristics: [String]?

The characteristics that describe the content of the language option.

var languageTag: String?

The abbreviated language code for the language option.

var languageOptionType: MPNowPlayingInfoLanguageOptionType

The type of language option.

enum MPNowPlayingInfoLanguageOptionType

The language option type to use for the Now Playing item.

### Retrieving a language option based on system preferences

func isAutomaticAudibleLanguageOption() -> Bool

Returns a Boolean value that determines whether to use the best audible language option based on the system preferences.

func isAutomaticLegibleLanguageOption() -> Bool

Returns a Boolean value that determines whether to use the best legible language option based on the system preferences.

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

class MPNowPlayingInfoLanguageOptionGroup

A grouped set of language options where only a single language option can be active at a time.

Language option characteristic constants

The constants for defining language characteristics.

