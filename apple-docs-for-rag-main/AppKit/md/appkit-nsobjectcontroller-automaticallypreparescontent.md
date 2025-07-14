

- AppKit
- NSObjectController
-  automaticallyPreparesContent 

Instance Property

# automaticallyPreparesContent

A Boolean that shows whether the receiver automatically creates and inserts new content objects automatically when loading from a nib file.

macOS

``` source
var automaticallyPreparesContent: Bool { get set }
```

## Discussion

If `flag` is true and the receiver is not using a managed object context, prepareContent() is used to create the content object. If `flag` is true and a managed object context is set, the initial content is fetched from the managed object context using the current fetch predicate. The default is false.

## See Also

### Managing content

var content: Any?

The receiver’s content object.

func prepareContent()

Typically overridden by subclasses that require additional control over the creation of new objects.

