

- UIKit
-  UIListContentConfiguration 

Structure

# UIListContentConfiguration

A content configuration for a list-based content view.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct UIListContentConfiguration
```

## Overview

A list content configuration describes the styling and content for an individual element that might appear in a list, like a cell, header, or footer. Using a list content configuration, you can obtain system default styling for a variety of different view states. You fill the configuration with your content, and then assign it directly to cells, headers, and footers in UICollectionView and UITableView, or to your own custom list content view (UIListContentView).

For views like cells, headers, and footers, use their defaultContentConfiguration() to get a list content configuration that has preconfigured default styling. Alternatively, you can create a list content configuration from one of the system default styles. After you get the configuration, you assign your content to it, customize any other properties, and assign it to your view as the current content configuration.

```
var content = cell.defaultContentConfiguration()

// Configure content.
content.image = UIImage(systemName: "star")
content.text = "Favorites"

// Customize appearance.
content.imageProperties.tintColor = .purple

cell.contentConfiguration = content
```

## Topics

### Creating default cell configurations

static func cell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell in a list.

static func subtitleCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in a list and contains subtitle text.

static func valueCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in a list and contains side-by-side value text.

static func sidebarCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell in a sidebar list.

static func sidebarSubtitleCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in a sidebar list and contains subtitle text.

static func accompaniedSidebarCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell in an accompanied sidebar list.

static func accompaniedSidebarSubtitleCell() -> UIListContentConfiguration

Creates the default configuration you use to style a cell that’s in an accompanied sidebar list and contains subtitle text.

### Creating header and footer configurations

static func plainHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a plain list.

static func plainFooter() -> UIListContentConfiguration

Creates the default configuration you use to style a footer in a plain list.

static func groupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a grouped list.

static func groupedFooter() -> UIListContentConfiguration

Creates the default configuration you use to style a footer in a grouped list.

static func prominentInsetGroupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a prominent header in an inset grouped list.

static func extraProminentInsetGroupedHeader() -> UIListContentConfiguration

Creates the default configuration you use to style an extra prominent header in an inset grouped list.

static func sidebarHeader() -> UIListContentConfiguration

Creates the default configuration you use to style a header in a sidebar list.

### Customizing content

var image: UIImage?

The image to display.

var text: String?

The primary text.

var attributedText: NSAttributedString?

An attributed variant of the primary text.

var secondaryText: String?

The secondary text.

var secondaryAttributedText: NSAttributedString?

An attributed variant of the secondary text.

### Customizing appearance

var imageProperties: UIListContentConfiguration.ImageProperties

Properties for configuring the image.

var textProperties: UIListContentConfiguration.TextProperties

Properties for configuring the primary text.

var secondaryTextProperties: UIListContentConfiguration.TextProperties

Properties for configuring the secondary text.

struct ImageProperties

Properties that affect the list content configuration’s image.

struct TextProperties

Properties that affect the list content configuration’s text.

### Customizing layout

var axesPreservingSuperviewLayoutMargins: UIAxis

A Boolean value that determines whether the content view preserves the layout margins that it inherits from its superview on the horizontal or vertical axes.

var directionalLayoutMargins: NSDirectionalEdgeInsets

The margins between the content and the edges of the content view.

var prefersSideBySideTextAndSecondaryText: Bool

A Boolean value that determines whether the configuration positions the text and secondary text side by side.

var imageToTextPadding: CGFloat

The padding between the image and text.

var textToSecondaryTextHorizontalPadding: CGFloat

The minimum horizontal padding between the text and secondary text.

var textToSecondaryTextVerticalPadding: CGFloat

The vertical padding between the text and secondary text.

### Instance Properties

var alpha: CGFloat

### Type Methods

static func footer() -> UIListContentConfiguration

static func header() -> UIListContentConfiguration

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- UIContentConfiguration

## See Also

### Content configurations

class UIListContentView

A content view for displaying list-based content.

protocol UIContentConfiguration

The requirements for an object that provides the configuration for a content view.

protocol UIContentView

The requirements for a content view that you create using a configuration.

