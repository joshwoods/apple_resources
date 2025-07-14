

- ActivityKit
- ActivityAttributes
-  previewContext(\_:isStale:viewKind:) 

Instance Method

# previewContext(\_:isStale:viewKind:)

Generates a preview for a Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
func previewContext(
    _ contentState: Self.ContentState,
    isStale: Bool = false,
    viewKind: ActivityPreviewViewKind
) -> some View
```

## Parameters 

`contentState`  

The dynamic content of the Live Activity.

`isStale`  

A Boolean that indicates whether the content of a Live Activity is out of date.

`viewKind`  

A value that determines which Live Activity presentation to render for this preview.

