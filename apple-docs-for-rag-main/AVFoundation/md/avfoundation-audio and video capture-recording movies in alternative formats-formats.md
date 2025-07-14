

- AVFoundation
- Audio and video capture
-  Recording movies in alternative formats 

Article

# Recording movies in alternative formats

Change the default format for capturing movie files.

## Overview

You use AVCaptureMovieFileOutput to capture QuickTime movie files, and the framework chooses the HEVC format by default on most iPhone and iPad models. However, you can change the default format in advance if you know you need a different format.

If your app shares the captured video using a system share sheet, the system automatically converts the video to a format thatʼs compatible with the destination device. However, if your app saves or shares captured video internally, for applications outside the system share sheet, you need to use a video-capture format thatʼs compatible with all target devices. This article shows you how to change the capture format dynamically, so that videos captured in your app begin in the desired format.

### Change the default capture format

You can change the default format at capture time by specifying it in the output settings for capturing movie files. Each capture device has a dictionary of settings that you adjust to control properties of the output movie file. For example, to capture video in H.264/MPEG-4 AVC, set the output settings key AVVideoCodecKey to h264, as the example below shows:

- Swift
- Objective-C

```
import AVFoundation

let movieFileOutput = // Your AVCaptureMovieFileOutput. //

if movieFileOutput.availableVideoCodecTypes.contains(.h264),
    let connection = movieFileOutput.connection(with: .video) {
    // Use the H.264 codec to encode the video.
    movieFileOutput.setOutputSettings([AVVideoCodecKey: AVVideoCodecType.h264], for: connection)
}
```

```
#import 

AVCaptureMovieFileOutput *movieFileOutput = // Your AVCaptureMovieFileOutput. //;

if ([movieFileOutput.availableVideoCodecTypes containsObject:AVVideoCodecTypeH264]) {
    AVCaptureConnection* connection = [movieFileOutput connectionWithMediaType:AVMediaTypeVideo];
    // Use the H.264 codec to encode the video.
    [movieFileOutput setOutputSettings:@{AVVideoCodecKey: AVVideoCodecTypeH264} forConnection:connection];
}
```

For a list of supported capture codecs, see AVVideoCodecType.

### Convert previously captured movie files

In addition to saving or sharing captured video using a different default format, you can also convert existing movie file content by generating a new movie file based on the contents of the existing file. For details on how, see Exporting video to alternative formats.

## See Also

### Related Documentation

static let h264: AVVideoCodecType

The H.264 video codec.

static let hevc: AVVideoCodecType

The HEVC video codec.

static let jpeg: AVVideoCodecType

The JPEG video codec.

static let proRes422: AVVideoCodecType

The Apple ProRes 422 video codec.

static let proRes4444: AVVideoCodecType

The Apple ProRes 4444 video codec.

### File capture

class AVCaptureMovieFileOutput

A capture output that records video and audio to a QuickTime movie file.

class AVCaptureAudioFileOutput

A capture output that records audio and saves the recorded audio to a file.

class AVCaptureFileOutput

The abstract superclass for capture outputs that can record captured data to a file.

protocol AVCaptureFileOutputDelegate

Methods for monitoring or controlling the output of a media file capture.

protocol AVCaptureFileOutputRecordingDelegate

Methods for responding to events that occur while recording captured media to a file.

