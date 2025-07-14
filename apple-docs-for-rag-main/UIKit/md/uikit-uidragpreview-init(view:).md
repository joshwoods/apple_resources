

- UIKit
- UIDragPreview
-  init(view:) 

Initializer

# init(view:)

Initializes a new drag item preview with a view, using the default appearance parameters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(view: UIView)
```

## Parameters 

`view`  

A UIView object representing the drag item.

## Return Value

A drag preview that is based on the specified view.

## Discussion

Use this method to display a drag item preview based on a view that you provide. The preview displays a snapshot of the provided view. Changes to the view don’t appear after the preview is shown, and the preview doesn’t change or move the view.

## See Also

### Initializing a drag item preview

init(view: UIView, parameters: UIDragPreviewParameters)

Initializes a new drag item preview with a view and with a set of appearance parameters.

convenience init(forURL: URL)

Initializes a new drag item preview with a URL.

convenience init(forURL: URL, title: String?)

Initializes a drag item preview with a URL and title.

