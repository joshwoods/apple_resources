

- AppKit
- NSFontCollection
- NSFontCollection.Visibility
-  user 

Type Property

# user

The font collection is visible to all processes and is stored persistently.

macOS

``` source
static var user: NSFontCollection.Visibility { get }
```

## See Also

### Visibility Options

static var process: NSFontCollection.Visibility

The font collection is visible within this process and is not persistent.

static var computer: NSFontCollection.Visibility

The font collection is visible to all users and is stored persistently.

