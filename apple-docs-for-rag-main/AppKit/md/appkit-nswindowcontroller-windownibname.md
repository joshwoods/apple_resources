

- AppKit
- NSWindowController
-  windowNibName 

Instance Property

# windowNibName

The name of the nib file that stores the window associated with the receiver.

macOS

``` source
@MainActor
var windowNibName: NSNib.Name? { get }
```

## Discussion

If init(windowNibPath:owner:) was used to initialize the instance, windowNibName contains the last path component with the “`.nib`” extension stripped off. If init(windowNibName:) or init(windowNibName:owner:) was used, NSWindowController contains the name without the “`.nib`” extension.

## See Also

### Getting Nib and Storyboard Information

var owner: AnyObject?

The owner of the nib file containing the window managed by the receiver.

var storyboard: NSStoryboard?

The storyboard file from which the window controller was loaded.

var windowNibPath: String?

The full path of the nib file that stores the window associated with the receiver.

