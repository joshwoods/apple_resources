

- AVFoundation
- AVAsset
-  hasProtectedContent Deprecated

Instance Property

# hasProtectedContent

A Boolean value that indicates whether the asset contains protected content.

iOS 4.2–16.0DeprecatediPadOS 4.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0Deprecated

``` source
var hasProtectedContent: Bool { get }
```

Deprecated

Load the value of hasProtectedContent asynchronously instead.

## Discussion

Assets that contain protected content may not be playable without successful authorization, even if the value of its isPlayable property is true.

