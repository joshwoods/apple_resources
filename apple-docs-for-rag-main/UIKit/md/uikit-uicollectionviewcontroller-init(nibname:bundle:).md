

- UIKit
- UICollectionViewController
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Returns a newly initialized view controller with the nib file in the specified bundle.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    nibName nibNameOrNil: String?,
    bundle nibBundleOrNil: Bundle?
)
```

## Parameters 

`nibNameOrNil`  

The name of the nib file to associate with the view controller. The nib file name shouldn’t contain any leading path information. If you specify `nil`, the nibName property is set to `nil`.

`nibBundleOrNil`  

The bundle in which to search for the nib file. This method looks for the nib file in the bundle’s language-specific project directories first, followed by the Resources directory.

## Return Value

A newly initialized UICollectionViewController object.

## Discussion

For more information on how to initialize a view controller from a nib file, see init(nibName:bundle:).

## See Also

### Creating a collection view controller

init(collectionViewLayout: UICollectionViewLayout)

Initializes a collection view controller and configures the collection view with the provided layout.

init?(coder: NSCoder)

Creates a collection view controller with the nib file in the specified bundle.

