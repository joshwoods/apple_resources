

- SwiftUI
-  SearchPresentationToolbarBehavior 

Structure

# SearchPresentationToolbarBehavior

A type that defines how the toolbar behaves when presenting search.

iOS 17.1+iPadOS 17.1+Mac Catalyst 17.1+macOS 14.1+tvOS 17.1+visionOS 1.0+watchOS 10.1+

``` source
struct SearchPresentationToolbarBehavior
```

## Overview

Use this type in combination with the searchPresentationToolbarBehavior(_:)

## Topics

### Getting toolbar behaviors

static var automatic: SearchPresentationToolbarBehavior

The automatic behavior.

static var avoidHidingContent: SearchPresentationToolbarBehavior

The avoid hiding content behavior.

## See Also

### Displaying toolbar content during search

func searchPresentationToolbarBehavior(SearchPresentationToolbarBehavior) -> some View

Configures the search toolbar presentation behavior for any searchable modifiers within this view.

