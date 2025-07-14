

- MapKit
- MKLookAroundViewController
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Creates a new LookAround view controller from the specified nib and bundle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
init(
    nibName nibNameOrNil: String?,
    bundle nibBundleOrNil: Bundle?
)
```

## Parameters 

`nibNameOrNil`  

The name of the nib file.

`nibBundleOrNil`  

The Bundle file.

## See Also

### Creating a LookAround controller

init?(coder: NSCoder)

Creates a new LookAround view controller object from a coder object provided by a storyboard or nib file.

init(scene: MKLookAroundScene)

Creates a new LookAround view controller with the specified scene.

