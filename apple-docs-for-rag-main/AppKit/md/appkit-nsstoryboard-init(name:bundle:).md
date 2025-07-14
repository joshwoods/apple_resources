

- AppKit
- NSStoryboard
-  init(name:bundle:) 

Initializer

# init(name:bundle:)

Creates a storyboard based on the named storyboard file in the specified bundle.

macOS 10.10+

``` source
convenience init(
    name: NSStoryboard.Name,
    bundle storyboardBundleOrNil: Bundle?
)
```

## Parameters 

`name`  

The name of the storyboard file, without the filename extension. This method raises an exception if this parameter’s value is `nil`.

`storyboardBundleOrNil`  

The bundle used to resolve references to resources, typically images, in the archived controllers represented in the storyboard file. If you specify `nil`, AppKit uses the app’s main bundle.

## Return Value

A new storyboard object.

## See Also

### Creating a Storyboard Object

class var main: NSStoryboard?

The app’s main storyboard.

typealias Name

The name of the storyboard file.

