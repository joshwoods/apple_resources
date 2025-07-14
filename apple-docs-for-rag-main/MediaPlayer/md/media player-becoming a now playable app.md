

- Media Player
-  Becoming a now playable app 

Sample Code

# Becoming a now playable app

Ensure your app is eligible to become the Now Playing app by adopting best practices for providing Now Playing info and registering for remote command center actions.

Download

iOS 12.2+iPadOS 12.2+macOS 10.14+tvOS 12.2+Xcode 14.3+

## Overview

Note

This sample code project is associated with WWDC 2019 session 501: Reaching the Big Screen with AirPlay 2.

### Configure the sample code project

Before you run the sample code project in Xcode:

- See the comments for the `NowPlayable` protocol in file `NowPlayable.swift`, to learn what settings and configuration you may want to customize for your use-case.

- Use the platform-specific `NowPlayableBehavior` class to implement your customizations to the standard behavior.

## See Also

### Now Playing information

class MPNowPlayingSession

An object that manages Now Playing information and remote commands for multiple players.

class MPNowPlayingInfoCenter

An object for setting the Now Playing information for media that your app plays.

class MPNowPlayingInfoLanguageOption

A set of interfaces for setting the language option for the Now Playing item.

class MPNowPlayingInfoLanguageOptionGroup

A grouped set of language options where only a single language option can be active at a time.

Language option characteristic constants

The constants for defining language characteristics.

