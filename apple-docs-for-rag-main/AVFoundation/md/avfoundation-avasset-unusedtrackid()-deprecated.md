

- AVFoundation
- AVAsset
-  unusedTrackID() Deprecated

Instance Method

# unusedTrackID()

Returns an identifier that no other tracks in the asset use.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func unusedTrackID() -> CMPersistentTrackID
```

Deprecated

Use findUnusedTrackID(completionHandler:) instead.

## Return Value

An unused CMPersistentTrackID value.

