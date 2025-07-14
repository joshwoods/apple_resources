

- Video Toolbox
-  kVTCompressionPropertyKey_ProfileLevel 

Global Variable

# kVTCompressionPropertyKey_ProfileLevel

The profile and level for the encoded bitstream.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_ProfileLevel: CFString
```

## Discussion

Available profiles and levels vary across formats and among video encoders. Video encoders should use standard keys where available, and follow standard patterns when standard keys are unavailable.

## Topics

### HEVC

let kVTProfileLevel_HEVC_Main_AutoLevel: CFString

let kVTProfileLevel_HEVC_Main10_AutoLevel: CFString

let kVTProfileLevel_HEVC_Main42210_AutoLevel: CFString

let kVTProfileLevel_HEVC_Monochrome10_AutoLevel: CFString

let kVTProfileLevel_HEVC_Monochrome_AutoLevel: CFString

### H.264

let kVTProfileLevel_H264_Baseline_1_3: CFString

let kVTProfileLevel_H264_Baseline_3_0: CFString

let kVTProfileLevel_H264_Baseline_3_1: CFString

let kVTProfileLevel_H264_Baseline_3_2: CFString

let kVTProfileLevel_H264_Baseline_4_0: CFString

let kVTProfileLevel_H264_Baseline_4_1: CFString

let kVTProfileLevel_H264_Baseline_4_2: CFString

let kVTProfileLevel_H264_Baseline_5_0: CFString

let kVTProfileLevel_H264_Baseline_5_1: CFString

let kVTProfileLevel_H264_Baseline_5_2: CFString

let kVTProfileLevel_H264_Baseline_AutoLevel: CFString

let kVTProfileLevel_H264_ConstrainedBaseline_AutoLevel: CFString

let kVTProfileLevel_H264_ConstrainedHigh_AutoLevel: CFString

let kVTProfileLevel_H264_Extended_5_0: CFString

let kVTProfileLevel_H264_Extended_AutoLevel: CFString

let kVTProfileLevel_H264_High_3_0: CFString

let kVTProfileLevel_H264_High_3_1: CFString

let kVTProfileLevel_H264_High_3_2: CFString

let kVTProfileLevel_H264_High_4_0: CFString

let kVTProfileLevel_H264_High_4_1: CFString

let kVTProfileLevel_H264_High_4_2: CFString

let kVTProfileLevel_H264_High_5_0: CFString

let kVTProfileLevel_H264_High_5_1: CFString

let kVTProfileLevel_H264_High_5_2: CFString

let kVTProfileLevel_H264_High_AutoLevel: CFString

let kVTProfileLevel_H264_Main_3_0: CFString

let kVTProfileLevel_H264_Main_3_1: CFString

let kVTProfileLevel_H264_Main_3_2: CFString

let kVTProfileLevel_H264_Main_4_0: CFString

let kVTProfileLevel_H264_Main_4_1: CFString

let kVTProfileLevel_H264_Main_4_2: CFString

let kVTProfileLevel_H264_Main_5_0: CFString

let kVTProfileLevel_H264_Main_5_1: CFString

let kVTProfileLevel_H264_Main_5_2: CFString

let kVTProfileLevel_H264_Main_AutoLevel: CFString

### MP4V

let kVTProfileLevel_MP4V_Simple_L0: CFString

let kVTProfileLevel_MP4V_Simple_L1: CFString

let kVTProfileLevel_MP4V_Simple_L2: CFString

let kVTProfileLevel_MP4V_Simple_L3: CFString

let kVTProfileLevel_MP4V_AdvancedSimple_L0: CFString

let kVTProfileLevel_MP4V_AdvancedSimple_L1: CFString

let kVTProfileLevel_MP4V_AdvancedSimple_L2: CFString

let kVTProfileLevel_MP4V_AdvancedSimple_L3: CFString

let kVTProfileLevel_MP4V_AdvancedSimple_L4: CFString

let kVTProfileLevel_MP4V_Main_L2: CFString

let kVTProfileLevel_MP4V_Main_L3: CFString

let kVTProfileLevel_MP4V_Main_L4: CFString

### H.263

let kVTProfileLevel_H263_Profile0_Level10: CFString

let kVTProfileLevel_H263_Profile0_Level45: CFString

let kVTProfileLevel_H263_Profile3_Level45: CFString

## See Also

### Bitstream Configuration

let kVTCompressionPropertyKey_PreserveAlphaChannel: CFString

A key that specifies whether to encode the alpha channel of input video frames.

let kVTCompressionPropertyKey_Depth: CFString

The pixel depth of the encoded video.

let kVTCompressionPropertyKey_H264EntropyMode: CFString

The entropy encoding mode for H.264 compression.

let kVTCompressionPropertyKey_HDRMetadataInsertionMode: CFString

let kVTCompressionPropertyKey_OutputBitDepth: CFString

