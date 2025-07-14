

- SwiftUI
-  ContentMarginPlacement 

Structure

# ContentMarginPlacement

The placement of margins.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ContentMarginPlacement
```

## Overview

Different views can support customizating margins that appear in different parts of that view. Use values of this type to customize those margins of a particular placement.

For example, use a scrollIndicators placement to customize the margins of scrollable view’s scroll indicators separately from the margins of a scrollable view’s content.

Use this type with the contentMargins(_:for:) modifier.

## Topics

### Getting the placement

static var automatic: ContentMarginPlacement

The automatic placement.

static var scrollContent: ContentMarginPlacement

The scroll content placement.

static var scrollIndicators: ContentMarginPlacement

The scroll indicators placement.

## See Also

### Setting margins

func contentMargins(CGFloat, for: ContentMarginPlacement) -> some View

Configures the content margin for a provided placement.

func contentMargins(_:_:for:)

Configures the content margin for a provided placement.

