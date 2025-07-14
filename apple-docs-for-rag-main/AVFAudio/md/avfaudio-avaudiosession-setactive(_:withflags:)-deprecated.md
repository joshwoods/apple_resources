

- AVFAudio
- AVAudioSession
-  setActive(\_:withFlags:) Deprecated

Instance Method

# setActive(\_:withFlags:)

Activates or deactivates your app’s audio session; provides flags for use by other audio sessions.

Mac Catalyst 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func setActive(
    _ active: Bool,
    withFlags flags: Int
) throws
```

Deprecated

Use setActive(_:options:) instead.

## Parameters 

`active`  

Use true to activate your app’s audio session or false to deactivate it.

`flags`  

A bitmapped value containing one or more flags.

## Discussion

If another app’s active audio session has higher priority than your app, and that other audio session doesn’t allow mixing with other apps, attempting to activate your audio session might fail.

