

- AppKit
- NSWindowController
-  windowNibPath 

Instance Property

# windowNibPath

The full path of the nib file that stores the window associated with the receiver.

macOS

``` source
@MainActor
var windowNibPath: String? { get }
```

## Discussion

If init(windowNibPath:owner:) was used to initialize the instance, this property contains the path. If init(windowNibName:) or init(windowNibName:owner:) was used, windowNibPath locates the nib in the file’s owner’s class’ bundle or in the application’s main bundle and returns the full path (or `nil` if it cannot be located). Subclasses can override this behavior to augment the search behavior, but probably ought to call `super` first.

## See Also

### Getting Nib and Storyboard Information

var owner: AnyObject?

The owner of the nib file containing the window managed by the receiver.

var storyboard: NSStoryboard?

The storyboard file from which the window controller was loaded.

var windowNibName: NSNib.Name?

The name of the nib file that stores the window associated with the receiver.

