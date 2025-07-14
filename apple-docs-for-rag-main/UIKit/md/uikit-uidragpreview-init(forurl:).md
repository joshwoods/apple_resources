

- UIKit
- UIDragPreview
-  init(forURL:) 

Initializer

# init(forURL:)

Initializes a new drag item preview with a URL.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
convenience init(forURL url: URL)
```

``` source
@MainActor
convenience init(for url: URL)
```

## Parameters 

`url`  

An Internet address referencing a remote resource, such as a webpage.

## Return Value

A drag preview for a URL.

## Discussion

This method creates a drag item preview of the URL. The URL preview is a one-line, textual representation that might not show the full URL string. Don’t use a file URL.

## See Also

### Initializing a drag item preview

convenience init(view: UIView)

Initializes a new drag item preview with a view, using the default appearance parameters.

init(view: UIView, parameters: UIDragPreviewParameters)

Initializes a new drag item preview with a view and with a set of appearance parameters.

convenience init(forURL: URL, title: String?)

Initializes a drag item preview with a URL and title.

