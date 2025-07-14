

- AVFoundation
- Media playback
-  Selecting Subtitles and Alternative Audio Tracks 

Article

# Selecting Subtitles and Alternative Audio Tracks

Extend your app’s appeal to users by adding subtitles and alternative audio tracks in their native language.

## Overview

As a developer, you want to make your apps accessible to as broad an audience as possible. One way for you to extend your app’s reach is to make it available to users in their native language as well as to provide support for users who have have hearing impairments or other accessibility needs. AVKit and AVFoundation simplify handling these concerns by providing built-in support for presenting subtitles and closed captions, and for selecting alternative audio and video tracks. If you’re building your own custom player or would like to present your own media-selection interface, use the features provided by AVFoundation’s AVMediaSelectionGroup and AVMediaSelectionOption classes.

### Retrieve the Available Media Options

`AVMediaSelectionOption` models an alternative audio, video, or text track contained within the source media. Media options are used to select alternative camera angles, present audio dubbed in a user’s native language, or display subtitles and closed captions. You determine which alternative media presentations are available by asynchronously loading and calling the asset’s availableMediaCharacteristicsWithMediaSelectionOptions property, which returns an array of strings indicating the available media characteristics. The possible values returned are audible (alternative audio tracks), visual (alternative video tracks), and legible (subtitles and closed captions).

After you’ve retrieved the array of available options, you call the asset’s mediaSelectionGroup(forMediaCharacteristic:) method, passing it the desired characteristic. This method returns the associated `AVMediaSelectionGroup` object, or `nil` if no groups exist for the specified characteristic.

`AVMediaSelectionGroup` acts as a container for a collection of mutually exclusive `AVMediaSelectionOption` objects. The following example shows how you retrieve an asset’s media-selection groups and display their available options:

```
for characteristic in asset.availableMediaCharacteristicsWithMediaSelectionOptions {
    print("\(characteristic)")

    // Retrieve the AVMediaSelectionGroup for the specified characteristic.
    if let group = asset.mediaSelectionGroup(forMediaCharacteristic: characteristic) {
        // Print its options.
        for option in group.options {
            print("  Option: \(option.displayName)")
        }
    }
}
```

The output for an asset containing audio and subtitle media options looks similar to the following:

```
[AVMediaCharacteristicAudible]
  Option: English
  Option: Spanish

[AVMediaCharacteristicLegible]
  Option: English
  Option: German
  Option: Spanish
  Option: French
```

### Select the Desired Media Option

After you’ve retrieved an `AVMediaSelectionGroup` object for a particular media characteristic and identified the desired `AVMediaSelectionOption` object, the next step is to select it. You select a media option by calling select(_:in:) on the active AVPlayerItem. For instance, to present the asset’s Spanish subtitle option, you could select it as follows:

```
if let group = asset.mediaSelectionGroup(forMediaCharacteristic: AVMediaCharacteristicLegible) {
    let locale = Locale(identifier: "es-ES")
    let options =
        AVMediaSelectionGroup.mediaSelectionOptions(from: group.options, with: locale)
    if let option = options.first {
        // Select Spanish-language subtitle option
        playerItem.select(option, in: group)
    }
}
```

Selecting a media option makes it immediately available for presentation. Selecting a subtitle or closed-caption option displays the associated text within the video display provided by AVPlayerViewController, AVPlayerView, and AVPlayerLayer. Selecting an alternative audio or video option replaces the currently presented media with the new selection’s media.

AVPlayer automatically selects media based on the user’s system preferences as its default behavior. To take control over when it makes media selections, disable the default behavior by setting the player’s appliesMediaSelectionCriteriaAutomatically value to false.

## See Also

### Media selection

class AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

class AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

class AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

class AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

class AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

