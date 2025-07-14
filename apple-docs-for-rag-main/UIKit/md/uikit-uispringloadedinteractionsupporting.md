

- UIKit
-  UISpringLoadedInteractionSupporting 

Protocol

# UISpringLoadedInteractionSupporting

The interface that determines if an object supports a spring-loaded interaction for drag and drop activities.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UISpringLoadedInteractionSupporting : NSObjectProtocol
```

## Topics

### Checking the spring-loaded interaction status

var isSpringLoaded: Bool

A Boolean value that specifies whether the object is participating in spring-loaded interaction for a drag and drop activity.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIAlertController
- UIBarButtonItem
- UIButton
- UICollectionView
- UISearchTab
- UISegmentedControl
- UITab
- UITabBar
- UITabBarItem
- UITabGroup
- UITableView

## See Also

### Spring-loaded interactions

protocol UISpringLoadedInteractionBehavior

The interface for specifying the behavior of a spring-loaded interaction.

class UISpringLoadedInteraction

An interaction object for configuring and controlling spring-loaded, user-driven navigation during a drag activity.

protocol UISpringLoadedInteractionContext

The interface an object implements to provide information about a spring-loaded interaction.

protocol UISpringLoadedInteractionEffect

The interface for providing visual styling to a spring-loaded interaction based on the interaction state.

