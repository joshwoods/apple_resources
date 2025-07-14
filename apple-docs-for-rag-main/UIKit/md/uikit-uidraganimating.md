

- UIKit
-  UIDragAnimating 

Protocol

# UIDragAnimating

The interface for providing custom animation alongside the system’s lift, drop, and cancellation animations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIDragAnimating : NSObjectProtocol
```

## Overview

You can use a UIDragAnimating object to animate your own changes to the preview displayed during system-provided drag and drop animations.

## Topics

### Adding animations

func addAnimations(() -> Void)

Adds an animation block for modifying a view animation while it’s running.

**Required**

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds an animation completion block to run when a view animation has ended.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UICollectionViewDropPlaceholderContext
- UITableViewDropPlaceholderContext

## See Also

### Drag sources

class UIDragItem

A representation of an underlying data item as a person drags it from one location to another.

protocol UIDragDropSession

The common interface for querying the state of both drag sessions and drop sessions.

protocol UIDragSession

The interface for configuring a drag session.

