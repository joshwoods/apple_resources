

- Audio Toolbox
- ScheduledAudioSlice
-  init(mTimeStamp:mCompletionProc:mCompletionProcUserData:mFlags:mReserved:mReserved2:mNumberFrames:mBufferList:) 

Initializer

# init(mTimeStamp:mCompletionProc:mCompletionProcUserData:mFlags:mReserved:mReserved2:mNumberFrames:mBufferList:)

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    mTimeStamp: AudioTimeStamp,
    mCompletionProc: ScheduledAudioSliceCompletionProc?,
    mCompletionProcUserData: UnsafeMutableRawPointer,
    mFlags: AUScheduledAudioSliceFlags,
    mReserved: UInt32,
    mReserved2: UnsafeMutableRawPointer?,
    mNumberFrames: UInt32,
    mBufferList: UnsafeMutablePointer
)
```

