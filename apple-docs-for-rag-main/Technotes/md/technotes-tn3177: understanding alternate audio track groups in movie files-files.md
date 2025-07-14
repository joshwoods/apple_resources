

- Technotes
-  TN3177: Understanding alternate audio track groups in movie files 

Article

# TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

## Overview

Movies recorded in QuickTime Movie files and MPEG-4 files by the Camera app on iPhone 16 and iPhone 16 Pro, and by spatial video captures on Apple Vision Pro, may have more than one audio track, containing the same recording in different formats. One track carries Spatial Audio and the other serves as a stereo fallback.

Movie files collect these tracks into alternate groups, from which at most one track should be used at a time.

## Alternate groups

Movies use alternate groups to describe multiple language audio tracks and subtitle tracks. Alternate groups can also indicate the relationship between stereo and surround audio tracks when they are recordings of the same audio source: only one should be played at a time.

A track association (also called a track reference) can indicate that the stereo track is a *fallback track* for the surround track. In general, the older and more compatible formats are fallbacks for the newer and more sophisticated formats.

The iPhone 16 series and Apple Vision Pro use a similar approach when capturing Spatial Audio, writing QuickTime Movie files with an alternate group containing:

- a stereo AAC track, and

- a Spatial Audio track.

The stereo track is associated as the fallback track for the Spatial Audio track.

Important

If your app examines or uses audio tracks directly, it should honor the relationship between tracks in an alternate group, and use no more than one track from any alternate group at one time. If you mix audio from different tracks in the same group, your app will produce incorrect audio.

## Enabled tracks

When you use AVAsset APIs to access tracks in a movies, each track in the asset reports an `isEnabled` property telling you whether the track is marked in the movie file as enabled or disabled.

For alternate groups, at most one of the tracks will be marked as enabled, indicating a default or expected track in the group. All other tracks in the group will be marked as disabled.

In the case of alternate groups with a Spatial Audio track, the stereo track is marked enabled, and the Spatial Audio track is marked disabled.

If your app examines or uses audio tracks directly, and you have no other specific processing requirements, you can simply skip disabled tracks. To test whether a track is enabled or disabled, use load(.isEnabled):

```
for track in try await asset.loadTracks(withMediaType: .audio) {
    if try await track.load(.isEnabled) {
        //...
    }
}
```

To query alternate track groups, use the trackGroups property.

Important

If your app currently iterates over audio tracks for custom processing without taking notice of whether the tracks are enabled or disabled, you should update it to do so.

Note

AVPlayer uses a more sophisticated strategy. It automatically enables the audio track appropriate for the current audio route and disables the others.

## Enabled state in movie file tracks

When you’re using AVFoundation, you can rely on its APIs for parsing and writing movie files.

If you have reasons to implement parsing and writing yourself, you’ll need to understand where to find the enabled and alternate group state of tracks in the movie file format, whether QuickTime File Format or ISO Base Media File Format (`ISOBMFF`) (ISO/IEC 14496-12:2020).

Note

`MP4` files are the best known member of the `ISOBMFF` family.

QuickTime Movie and `ISOBMFF` files both carry audiovisual media. The QuickTime File Format and `ISOBMFF` are very similar, as the latter was based upon the former. The format organization of QuickTime Movie files uses structures called “atoms”. `ISOBMFF` files uses many of the same structures but calls them “boxes”. You can find descriptions of “Track atom” and “TrackBox”, for instance, by reading the respective specifications.

In QuickTime Movie files, the enabled state of a QuickTime Movie track is stored as a single bit flag (`0x000001`) in the 3-byte `Flags` field of the Track header atom. In the QuickTime File Format specification this flag is called Track enabled. If this bit is set to `1`, the track is enabled. Otherwise, when it is `0`, the track is disabled.

For MPEG-4 (or more generally `ISOBMFF`) files, the enabled state is carried in the 3-byte `flags` field of the `TrackHeaderBox`. The `track_enabled` flag (`0x000001`) is used to mark the track as enabled. A value of `0` in this position disables the track.

## Alternate group state in movie file tracks

Each movie track can optionally be associated with an alternate group. Typically, only tracks of a particular kind or category will be in the same alternate group. For example, one alternate group might contain only audio tracks. Another alternate group might contain only subtitle or closed caption tracks.

A track’s alternate group is signaled using a 16-bit integer used to associate tracks.

- In QuickTime Movie files, the Track header atom carries a 16-bit integer Alternate group field.

- In `ISOBMFF`, the `TrackHeaderBox` `ISOBMFF` carries a 16-bit integer `alternate_group` field.

A value of `0` indicates the track is not a member of an alternate group. A non-zero value in one track can be matched to the same value in other tracks to identify alternate group membership.

Note

If more than one audio or video track is present in an alternate group, their `track_enabled` flags, as described above, indicate the default choice of track from the group to be presented. The ordering of their serialization in the file should not be considered significant.

## Revision History

- **2024-09-26** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

