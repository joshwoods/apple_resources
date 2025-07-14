

- UIKit
-  UIPreviewActionItem 

Protocol

# UIPreviewActionItem

A set of methods that defines the styles you can apply to peek quick actions and peek quick action groups, and defines a read-only accessor for the user-visible title of a peek quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
protocol UIPreviewActionItem : NSObjectProtocol
```

## Overview

Important

Don’t adopt this protocol in custom classes.

The UIPreviewActionItem protocol is adopted by the UIPreviewAction and UIPreviewActionGroup classes.

## Topics

### Accessing peek quick action properties

var title: String

The peek quick action item’s title.

**Required**

### Constants

enum Style

The style for a peek quick action.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIPreviewAction
- UIPreviewActionGroup

## See Also

### 3D Touch interactions

class UIPreviewInteraction

A class that registers a view to provide a custom user experience in response to 3D Touch interactions.

protocol UIPreviewInteractionDelegate

A set of methods for communicating the progress of a preview interaction.

