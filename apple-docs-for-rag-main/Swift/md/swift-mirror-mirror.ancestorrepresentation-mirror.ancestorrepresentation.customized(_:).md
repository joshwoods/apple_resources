

- Swift
- Mirror
- Mirror.AncestorRepresentation
-  Mirror.AncestorRepresentation.customized(\_:) 

Case

# Mirror.AncestorRepresentation.customized(\_:)

Uses the nearest ancestor’s implementation of `customMirror` to create a mirror for that ancestor.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case customized(() -> Mirror)
```

## Discussion

Other classes derived from such an ancestor are given a default mirror. The payload for this option should always be `{ super.customMirror }`:

```
var customMirror: Mirror {
    return Mirror(
        self,
        children: ["someProperty": self.someProperty],
        ancestorRepresentation: .customized({ super.customMirror })) // 

