

- Audio Toolbox
- AUMessageChannel
-  callHostBlock 

Instance Property

# callHostBlock

A callback for the audio unit to send a message to the host.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional var callHostBlock: CallHostBlock? { get set }
```

## Discussion

The host must set a block on this property to use it.

