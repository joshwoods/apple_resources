

- SwiftUI
-  NavigationSplitViewColumn 

Structure

# NavigationSplitViewColumn

A view that represents a column in a navigation split view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct NavigationSplitViewColumn
```

## Overview

A NavigationSplitView collapses into a single stack in some contexts, like on iPhone or Apple Watch. Use this type with the `preferredCompactColumn` parameter to control which column of the navigation split view appears on top of the collapsed stack.

## Topics

### Getting a column

static var sidebar: NavigationSplitViewColumn

static var content: NavigationSplitViewColumn

static var detail: NavigationSplitViewColumn

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

