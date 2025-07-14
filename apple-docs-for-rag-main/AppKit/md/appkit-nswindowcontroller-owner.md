

- AppKit
- NSWindowController
-  owner 

Instance Property

# owner

The owner of the nib file containing the window managed by the receiver.

macOS

``` source
@MainActor
weak var owner: AnyObject? { get }
```

## Discussion

The owner of the nib file containing the window managed by the receiver is usually `self`, but it can be the receiver’s document or some other object.

## See Also

### Getting Nib and Storyboard Information

var storyboard: NSStoryboard?

The storyboard file from which the window controller was loaded.

var windowNibName: NSNib.Name?

The name of the nib file that stores the window associated with the receiver.

var windowNibPath: String?

The full path of the nib file that stores the window associated with the receiver.

