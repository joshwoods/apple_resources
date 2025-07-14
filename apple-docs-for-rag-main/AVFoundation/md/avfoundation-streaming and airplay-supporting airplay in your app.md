

- AVFoundation
- Streaming and AirPlay
-  Supporting AirPlay in your app 

Article

# Supporting AirPlay in your app

Set up your app to use AirPlay to send content wirelessly.

## Overview

AirPlay enables you to send content wirelessly from an Apple device to an Apple TV or AirPlay-enabled speaker. AirPlay provides enhanced support for wireless audio distribution, including the ability to send content to multiple AirPlay-enabled speakers.

### Identify the audio type the app plays

In iOS, tvOS, and watchOS, set your audio session’s route-sharing policy to `.longForm`. Long-form audio is anything other than system sounds, such as music, audiobooks, or podcasts. This setting identifies the audio that an app plays, such as in the following example.

```
let audioSession = AVAudioSession.sharedInstance()
try audioSession.setCategory(.playback, 
                             mode: .default, 
                             policy: .longFormAudio)
```

### Add an AirPlay picker

Add AVRoutePickerView to your view hierarchy to include an AirPlay picker in your app. The picker provides users with a list of potential AirPlay devices they can use with your app. To control when to show the picker, use AVRouteDetector to identify the state of the route detector.

### Add a media player

Use APIs to customize your AirPlay adoption with Media Player integration. If you use MPRemoteCommandCenter, you can receive remote commands. If you use MPNowPlayingInfoCenter, you can inform the system metadata about the track that’s playing on the device.

### Configure an app for fast streaming

Adopt one of two playback API sets that take advantage of the enhanced buffering in AirPlay:

- For simple enhanced buffering, use AVPlayer or AVQueuePlayer. This works well for video content. For more information, see Implementing simple enhanced buffering for your content.

- For more flexibility with enhanced buffering, use AVSampleBufferAudioRenderer and AVSampleBufferRenderSynchronizer. This option is better for apps that require control over I/O, perform preprocessing on their media data, or have a DRM model that AVPlayer doesn’t support. For more information, see Implementing flexible enhanced buffering for your content.

