

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatFlags
-  FormatFlagIsNonInterleaved 

Enumeration Case

# FormatFlagIsNonInterleaved

A flag to indicate whether the channels interleave their samples in the data.

DriverKit 21.0+

``` source
FormatFlagIsNonInterleaved
```

## Discussion

Set this flag if the each channel lays out its samples contiguously, with the channels layed out end to end. Clear this flag if each frame lays out its samples contiguously, with the frames layed out end to end.

## See Also

### Channel Layout Flags

LinearPCMFormatFlagIsNonInterleaved

A flag to indicate whether PCM channels interleave their samples in the data.

