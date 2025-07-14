

- UIKit
- UIDragPreview
-  init(forURL:title:) 

Initializer

# init(forURL:title:)

Initializes a drag item preview with a URL and title.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
convenience init(
    forURL url: URL,
    title: String?
)
```

``` source
@MainActor
convenience init(
    for url: URL,
    title: String?
)
```

## Parameters 

`url`  

An Internet address referencing a remote resource, such as a webpage.

`title`  

A title for the URL.

## Return Value

A drag preview for a URL that has a title.

## Discussion

This method creates a two-line drag item preview, with the title displayed on the first line. The second line is a textual representation of the URL that might not show the full URL string. Don’t use a file URL. Passing `nil` for the title is the same as calling init(forURL:).

## See Also

### Initializing a drag item preview

convenience init(view: UIView)

Initializes a new drag item preview with a view, using the default appearance parameters.

init(view: UIView, parameters: UIDragPreviewParameters)

Initializes a new drag item preview with a view and with a set of appearance parameters.

convenience init(forURL: URL)

Initializes a new drag item preview with a URL.

