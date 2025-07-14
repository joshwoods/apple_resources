

- UIKit
- UITableViewHeaderFooterView
-  contentView 

Instance Property

# contentView

The content view of the header or footer.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentView: UIView { get }
```

## Mentioned in 

Adding headers and footers to table sections

## Discussion

To create your header or footer content, you add subviews to the view in this property. Your custom subviews represent the main content of your header or footer. Be sure to configure all subviews.

## See Also

### Managing the content

func defaultContentConfiguration() -> UIListContentConfiguration

Retrieves a default list content configuration for the view’s style.

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the view.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the view automatically updates its content configuration when its state changes.

