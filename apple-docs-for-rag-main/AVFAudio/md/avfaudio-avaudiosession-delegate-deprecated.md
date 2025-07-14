

- AVFAudio
- AVAudioSession
-  delegate Deprecated

Instance Property

# delegate

The delegate object for the audio session.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
unowned(unsafe) var delegate: (any AVAudioSessionDelegate)? { get set }
```

Deprecated

Use the notifications described in the Handling interruptions section of this class instead.

## Discussion

The delegate object must implement the protocol described in AVAudioSessionDelegate.

## See Also

### Responding to audio session changes

protocol AVAudioSessionDelegate

A protocol that defines responses to changes in state for the audio session.

Deprecated

