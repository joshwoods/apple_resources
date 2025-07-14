

- Audio Toolbox
-  kAudioSessionIncompatibleCategory 

Global Variable

# kAudioSessionIncompatibleCategory

The specified audio session category cannot be used for the attempted audio operation. For example, you attempted to play or record audio with the audio session category set to `kAudioSessionCategory_AudioProcessing`.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
var kAudioSessionIncompatibleCategory: Int { get }
```

## See Also

### Constants

var kAudioSessionNoError: Int

No error has occurred.

var kAudioSessionNotInitialized: Int

An Audio Session function was called without first initializing the session. To avoid this error, call the `AudioSessionInitialize` function before attempting to use the session.

var kAudioSessionAlreadyInitialized: Int

The `AudioSessionInitialize` function was called more than once during the lifetime of your application.

var kAudioSessionInitializationError: Int

There was an error during audio session initialization.

var kAudioSessionUnsupportedPropertyError: Int

The audio session property is not supported.

var kAudioSessionBadPropertySizeError: Int

The size of the audio session property data was not correct.

var kAudioSessionNotActiveError: Int

The audio operation failed because your application’s audio session was not active.

var kAudioServicesNoHardwareError: Int

The audio operation failed because the device has no audio input available.

var kAudioSessionNoCategorySet: Int

The audio operation failed because it requires the audio session to have an explicitly-set category, but none was set. To use a hardware codec you must explicitly initialize the audio session and explicitly set an audio session category.

var kAudioSessionUnspecifiedError: Int

An unspecified audio session error has occurred. This typically results from the audio system being in an inconsistent state.

