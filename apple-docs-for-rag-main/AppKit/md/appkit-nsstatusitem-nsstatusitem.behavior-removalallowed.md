

- AppKit
- NSStatusItem
- NSStatusItem.Behavior
-  removalAllowed 

Type Property

# removalAllowed

A status item that allows interactive removal.

macOS 10.12+

``` source
static var removalAllowed: NSStatusItem.Behavior { get }
```

## Discussion

Status items with this behavior allow interactive removal from the menu bar. Upon removal, the item’s isVisible property changes to false. This change is observable using key-value observation.

## See Also

### Behaviors

static var terminationOnRemoval: NSStatusItem.Behavior

A status item that quits the application upon removal.

