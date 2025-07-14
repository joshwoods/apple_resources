

- UIKit
- UITargetedDragPreview
-  init(forURL:target:) 

Initializer

# init(forURL:target:)

Initializes a new targeted drag item preview with a URL and a drag item preview.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
convenience init(
    forURL url: URL,
    target: UIDragPreviewTarget
)
```

``` source
@MainActor
convenience init(
    for url: URL,
    target: UIDragPreviewTarget
)
```

## Parameters 

`url`  

An Internet address referencing a remote resource, such as a webpage.

`target`  

A drag item preview target.

## Return Value

A targeted drag preview for a URL based on the drag item preview target.

## Discussion

This method creates a targeted drag item preview of the URL. The URL preview is a one-line, textual representation that might not show the full URL string. Don’t use a file URL.

## See Also

### Initializing a targeted drag item preview

convenience init(forURL: URL, title: String?, target: UIDragPreviewTarget)

Initializes a new targeted drag item preview with a URL, a title, and a drag item preview.

