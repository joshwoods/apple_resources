

- AppKit
- NSStoryboard
-  main 

Type Property

# main

The app’s main storyboard.

macOS 10.13+

``` source
class var main: NSStoryboard? { get }
```

## Discussion

The name of the main storyboard is stored in the NSMainStoryboardFile key of the app’s `Info.plist` file.

## See Also

### Creating a Storyboard Object

convenience init(name: NSStoryboard.Name, bundle: Bundle?)

Creates a storyboard based on the named storyboard file in the specified bundle.

typealias Name

The name of the storyboard file.

