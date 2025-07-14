

- UIKit
- UICollectionViewController
-  init(collectionViewLayout:) 

Initializer

# init(collectionViewLayout:)

Initializes a collection view controller and configures the collection view with the provided layout.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(collectionViewLayout layout: UICollectionViewLayout)
```

## Parameters 

`layout`  

The layout object to associate with the collection view. The layout controls how the collection view presents its cells and supplementary views.

## Return Value

An initialized `UICollectionViewController` object or `nil` if the object could not be created.

## See Also

### Creating a collection view controller

init(nibName: String?, bundle: Bundle?)

Returns a newly initialized view controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a collection view controller with the nib file in the specified bundle.

