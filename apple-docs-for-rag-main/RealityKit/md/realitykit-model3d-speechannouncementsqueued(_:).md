

- RealityKit
- Model3D
-  speechAnnouncementsQueued(\_:) 

Instance Method

# speechAnnouncementsQueued(\_:)

Controls whether to queue pending announcements behind existing speech rather than interrupting speech in progress.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func speechAnnouncementsQueued(_ value: Bool = true) -> some View
```

## Parameters 

`value`  

A Boolean value that determines if VoiceOver speaks changes to text immediately or enqueues them behind existing speech. Defaults to `true`.

## Discussion

Use this modifier when you want affect the order in which the accessibility system delivers spoken text. Announcements can occur automatically when the label or value of an accessibility element changes.

