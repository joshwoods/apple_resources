

- Video Toolbox
-  kVTCompressionPropertyKey_MultiPassStorage 

Global Variable

# kVTCompressionPropertyKey_MultiPassStorage

A property key that enables multipass compression and provides storage for encoder private data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MultiPassStorage: CFString
```

## Discussion

Some video encoders support multipass encoding. To determine whether a VTCompressionSession supports multipass encoding, you can inspect the dictionary returned by VTSessionCopySupportedPropertyDictionary(_:supportedPropertyDictionaryOut:) to see if it contains kVTCompressionPropertyKey_MultiPassStorage.

To enable multipass encoding, set the kVTCompressionPropertyKey_MultiPassStorage property to a VTMultiPassStorage object, which you can create by calling VTMultiPassStorageCreate(allocator:fileURL:timeRange:options:multiPassStorageOut:). Then make one or more passes over the source frames. Bracket each pass with a call to VTCompressionSessionBeginPass(_:flags:_:) at the beginning and VTCompressionSessionEndPass(_:furtherPassesRequestedOut:_:) at the end.

In the first pass of multipass encoding, call VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:) for every source frame (just as in single-pass encoding). At the end of every pass, call VTCompressionSessionEndPass(_:furtherPassesRequestedOut:_:). This may take some time as the video encoder determines whether it can improve the encoding by performing another pass. If the user cancels encoding during this time, call VTCompressionSessionInvalidate(_:) to interrupt the processing. VTCompressionSessionEndPass(_:furtherPassesRequestedOut:_:) indicates through the `furtherPassesRequestedOut` argument whether the video encoder has requested another pass. There is no particular limit on the number of passes the video encoder may request, but the client is free to disregard this request and use the last-emitted set of frames.

If `furtherPassesRequestedOut` is set to true and you want to perform another pass, call VTCompressionSessionGetTimeRangesForNextPass(_:timeRangeCountOut:timeRangeArrayOut:) to determine the time ranges for the next pass. Only the source frames within these time ranges need to be passed to VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:); the video encoder is satisfied with the already-emitted compressed frames outside these ranges, and they can be kept for the final output.

In second and successive passes, you must pass identical source frames, frame properties, and timestamps to VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:) as in the first pass, with the exception that frames not in the requested time ranges should be skipped.

You can create and use a VTFrameSilo object to merge sequences of compressed frames across passes during multipass encoding.

