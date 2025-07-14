

- AppKit
- NSObjectController
-  prepareContent() 

Instance Method

# prepareContent()

Typically overridden by subclasses that require additional control over the creation of new objects.

macOS

``` source
func prepareContent()
```

## Discussion

Subclasses that implement this method are responsible for creating the new content object and setting it as the receiver’s content object. This method is only called if automaticallyPreparesContent has been set to true.

## See Also

### Managing content

var content: Any?

The receiver’s content object.

var automaticallyPreparesContent: Bool

A Boolean that shows whether the receiver automatically creates and inserts new content objects automatically when loading from a nib file.

