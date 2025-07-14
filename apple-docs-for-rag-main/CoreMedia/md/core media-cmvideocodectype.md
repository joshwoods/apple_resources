

- Core Media
-  CMVideoCodecType 

Type Alias

# CMVideoCodecType

A video codec type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMVideoCodecType = FourCharCode
```

## Discussion

Certain codec types are also pixel formats.

There is no “kCMVideoCodecType_Raw”; you should use the appropriate pixel format type as the codec type.

## Topics

### Constants

var kCMVideoCodecType_422YpCbCr8: CMVideoCodecType

A type that identifies a component with the format of Y’CbCr 8-bit 4:2:2 ordered Cb Y’0 Cr Y’1.

var kCMVideoCodecType_Animation: CMVideoCodecType

A type that identifies the apple animation format.

var kCMVideoCodecType_Cinepak: CMVideoCodecType

A type that identifies the cinepak format.

var kCMVideoCodecType_JPEG: CMVideoCodecType

A type that identifies the Joint Photographic Experts Group (JPEG) format.

var kCMVideoCodecType_JPEG_OpenDML: CMVideoCodecType

A type that identifies the JPEG format with Open-DML extensions.

var kCMVideoCodecType_SorensonVideo: CMVideoCodecType

A type that identifies the sorenson video format.

var kCMVideoCodecType_SorensonVideo3: CMVideoCodecType

A type that identifies the sorenson 3 video format.

var kCMVideoCodecType_H263: CMVideoCodecType

A type that identifies the ITU-T H.263 format.

var kCMVideoCodecType_H264: CMVideoCodecType

A type that identifies the ITU-T H.264 format.

var kCMVideoCodecType_MPEG4Video: CMVideoCodecType

A type that identifies the Moving Picture Experts Group (MPEG) MPEG-4 Part 2 video format.

var kCMVideoCodecType_MPEG2Video: CMVideoCodecType

A type that identifies the MPEG-2 video format.

var kCMVideoCodecType_MPEG1Video: CMVideoCodecType

A type that identifies the MPEG-1 video format.

var kCMVideoCodecType_DVCNTSC: CMVideoCodecType

A type that identifies the DV NTSC format.

var kCMVideoCodecType_DVCPAL: CMVideoCodecType

A type that identifies the DV PAL format.

var kCMVideoCodecType_DVCProPAL: CMVideoCodecType

A type that identifies the Panasonic DVCPro PAL format.

var kCMVideoCodecType_DVCPro50NTSC: CMVideoCodecType

A type that identifies the Panasonic DVCPro-50 NTSC format.

var kCMVideoCodecType_DVCPro50PAL: CMVideoCodecType

A type that identifies the Panasonic DVCPro-50 PAL format.

var kCMVideoCodecType_DVCPROHD720p60: CMVideoCodecType

A type that identifies the Panasonic DVCPro-HD 720p60 format.

var kCMVideoCodecType_DVCPROHD720p50: CMVideoCodecType

A type that identifies the Panasonic DVCPro-HD 720p50 format.

var kCMVideoCodecType_DVCPROHD1080i60: CMVideoCodecType

A type that identifies the Panasonic DVCPro-HD 1080i60 format.

var kCMVideoCodecType_DVCPROHD1080i50: CMVideoCodecType

A type that identifies the Panasonic DVCPro-HD 1080i50 format.

var kCMVideoCodecType_DVCPROHD1080p30: CMVideoCodecType

A type that identifies the Panasonic DVCPro-HD 1080p30 format.

var kCMVideoCodecType_DVCPROHD1080p25: CMVideoCodecType

A type that identifies the Panasonic DVCPro-HD 1080p25 format.

## See Also

### Data Types

struct CMVideoDimensions

A structure that represents video dimensions.

typealias CMAudioFormatDescriptionMask

A type for mask bits that represent parts of an audio format description.

typealias CMMediaType

Constants that represent media types.

typealias CMAudioCodecType

An audio codec type.

typealias CMTextDisplayFlags

An integer value that describes the display mode flags for text media.

typealias CMTextJustificationValue

An integer value that describes the justification modes for text media.

Media Type Constants

Constants that represent media types.

Muxed Stream Types

Constants that represent muxed stream types.

Audio Codec Types

Constants that represent audio codec types.

