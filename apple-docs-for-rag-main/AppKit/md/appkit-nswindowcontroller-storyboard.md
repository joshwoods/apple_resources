

- AppKit
- NSWindowController
-  storyboard 

Instance Property

# storyboard

The storyboard file from which the window controller was loaded.

macOS 10.10+

``` source
@MainActor
var storyboard: NSStoryboard? { get }
```

## Discussion

The value of this property is `nil` if the window controller was not loaded from a storyboard.

## See Also

### Getting Nib and Storyboard Information

var owner: AnyObject?

The owner of the nib file containing the window managed by the receiver.

var windowNibName: NSNib.Name?

The name of the nib file that stores the window associated with the receiver.

var windowNibPath: String?

The full path of the nib file that stores the window associated with the receiver.

