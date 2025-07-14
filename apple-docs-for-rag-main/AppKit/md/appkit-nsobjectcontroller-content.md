

- AppKit
- NSObjectController
-  content 

Instance Property

# content

The receiver’s content object.

macOS

``` source
var content: Any? { get set }
```

## See Also

### Managing content

var automaticallyPreparesContent: Bool

A Boolean that shows whether the receiver automatically creates and inserts new content objects automatically when loading from a nib file.

func prepareContent()

Typically overridden by subclasses that require additional control over the creation of new objects.

