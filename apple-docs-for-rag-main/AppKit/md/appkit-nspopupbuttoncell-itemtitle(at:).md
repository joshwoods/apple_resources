

- AppKit
- NSPopUpButtonCell
-  itemTitle(at:) 

Instance Method

# itemTitle(at:)

Returns the title of the item at the specified index.

macOS

``` source
@MainActor
func itemTitle(at index: Int) -> String
```

## Parameters 

`index`  

The index of the item you want.

## Return Value

The title of the item, or an empty string if no item exists at the specified index.

## See Also

### Related Documentation

func item(at: Int) -> NSMenuItem?

Returns the menu item at the specified index.

### Title conveniences

var itemTitles: [String]

An array of `NSString` objects containing the titles of every item in the menu.

var titleOfSelectedItem: String?

The title of the item last selected by the user.

