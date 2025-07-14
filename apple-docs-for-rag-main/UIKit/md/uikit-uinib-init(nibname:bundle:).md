

- UIKit
- UINib
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Returns a nib object from the nib file in the specified bundle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(
    nibName name: String,
    bundle bundleOrNil: Bundle?
)
```

## Parameters 

`name`  

The name of the nib file, without any leading path information.

`bundleOrNil`  

The bundle in which to search for the nib file. If you specify `nil`, this method looks for the nib file in the main bundle.

## Return Value

The initialized UINib object. An exception is thrown if there were errors during initialization or the nib file could not be located.

## Discussion

The UINib object looks for the nib file in the bundle’s language-specific project directories first, followed by the `Resources` directory.

## See Also

### Creating a nib object

init(data: Data, bundle: Bundle?)

Creates a nib object from nib data stored in memory.

