

- UIKit
- UITargetedDragPreview
-  init(forURL:title:target:) 

Initializer

# init(forURL:title:target:)

Initializes a new targeted drag item preview with a URL, a title, and a drag item preview.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
convenience init(
    forURL url: URL,
    title: String?,
    target: UIDragPreviewTarget
)
```

``` source
@MainActor
convenience init(
    for url: URL,
    title: String?,
    target: UIDragPreviewTarget
)
```

## Parameters 

`url`  

An Internet address referencing a remote resource, such as a webpage.

`title`  

A title for the URL.

`target`  

A drag item preview target.

## Return Value

A drag preview for a URL with a title based on the specified drag item preview target.

## Discussion

This method creates a two-line drag item preview, with the title displayed on the first line. The second line is a textual representation of the URL that might not show the full URL string. Don’t use a file URL. Passing `nil` for the title is the same as calling init(forURL:target:).

## See Also

### Initializing a targeted drag item preview

convenience init(forURL: URL, target: UIDragPreviewTarget)

Initializes a new targeted drag item preview with a URL and a drag item preview.

