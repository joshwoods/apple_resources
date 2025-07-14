

- Updates
-  AVFoundation updates 

Article

# AVFoundation updates

Learn about important changes to AVFoundation.

## Overview

Browse notable changes in AVFoundation.

## June 2024

### Assets

- Preserve HDR data when generating images with `AVAssetImageGenerator` by setting the value of its dynamicRangePolicy property to match the source video.

- Export media asynchronously using the export(to:as:isolation:) method of AVAssetExportSession. You can monitor the progress of an export by calling the states(updateInterval:) method and awaiting its results.

- Determine whether an AVURLAsset decodes its data using a Media Extension by inspecting its mediaExtensionProperties property.

### Camera

- Show your camera app on the Lock Screen by adopting the LockedCameraCapture framework.

- Capture photos in constant color by configuring a photo output’s isConstantColorEnabled property.

- Continue background audio playback while performing audio and video capture by enabling a capture session’s configuresApplicationAudioSessionToMixWithOthers property.

- Pause and resume video recording in iOS when using AVCaptureFileOutput.

- Support enhanced video stabilization using AVCaptureVideoStabilizationMode.cinematicExtendedEnhanced.

- Configure a capture device to automatically adjust its frame rate based on lighting conditions by enabling its isAutoVideoFrameRateEnabled property.

- Configure a capture device to replace background content in macOS by enabling its isBackgroundReplacementEnabled property.

### Playback

- Build playback apps using the latest Swift Concurrency features due to enhanced Sendable adoption throughout the playback APIs.

- Capture performance and playback metrics using AVMetrics.

- Receive rendered captions for the currently playing media using AVPlayerItemRenderedLegibleOutput.

- Simplify handling of interstitial content by using AVPlayerItemIntegratedTimeline.

- Send Common Media Client Data (CMCD) as HTTP headers by enabling the new sendsCommonMediaClientDataAsHTTPHeaders property on AVAssetResourceLoader.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

Core Location updates

Learn about important changes to Core Location.

