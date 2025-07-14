

- TVMLKit
-  TVInterfaceCreating Deprecated

Protocol

# TVInterfaceCreating

A protocol that defines methods used to create views and view controllers.

tvOS 9.0–18.0Deprecated

``` source
protocol TVInterfaceCreating : NSObjectProtocol
```

Deprecated

Please use SwiftUI or UIKit

## Mentioned in 

Creating TVML Elements

## Overview

This protocol contains methods used to create views and view controllers from a TVViewElement.

## Topics

### Retrieving Resource Information

func resourceImage(name: String) -> UIImage?

Returns the image for the given resource

func resourceURL(name: String) -> URL?

Returns a URL for the given resource.

### Updating View Information

func makeViewController(element: TVViewElement, existingViewController: UIViewController?) -> UIViewController?

Returns a view controller for a view element.

func makeView(element: TVViewElement, existingView: UIView?) -> UIView?

Returns a view for a view element.

func collectionViewCellClass(for: TVViewElement) -> AnyClass?

Returns a collection view cell for the specified element.

func playerViewController(for: TVPlayer) -> UIViewController?

Returns the custom player user interface for a custom player.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- TVInterfaceFactory

## See Also

### Views and View Controllers

class TVViewElement

A representation of a read-only DOM node.

Deprecated

class TVInterfaceFactory

A factory for the creation of views and view controllers.

Deprecated

class TVBrowserViewController

A view controller that presents content in a browsable, full-screen format.

class TVDocumentViewController

A view controller that represents a TVMLKit document.

Deprecated

