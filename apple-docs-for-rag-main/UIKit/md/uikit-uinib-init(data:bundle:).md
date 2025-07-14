

- UIKit
- UINib
-  init(data:bundle:) 

Initializer

# init(data:bundle:)

Creates a nib object from nib data stored in memory.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(
    data: Data,
    bundle bundleOrNil: Bundle?
)
```

## Parameters 

`data`  

A block of memory that contains nib data.

`bundleOrNil`  

The bundle in which to search for resources referenced by the nib. If you specify `nil`, this method looks for the nib file in the main bundle.

## Return Value

The initialized UINib object. An exception is thrown if there were errors during initialization or the nib data could not be located.

## Discussion

The UINib object looks for the nib file in the bundle’s language-specific project directories first, followed by the `Resources` directory.

The preferred mechanism for instantiating UINib objects is with init(nibName:bundle:). A UINib object instantiated using init(data:bundle:) can’t release the cached data under low memory conditions. Your app should prepare to release the UINib object and the data under low memory conditions, recreating both the next time the app needs to instantiate the nib.

## See Also

### Creating a nib object

init(nibName: String, bundle: Bundle?)

Returns a nib object from the nib file in the specified bundle.

