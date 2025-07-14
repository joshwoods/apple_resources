

- AppKit
- NSHelpManager
-  openHelpAnchor(\_:inBook:) 

Instance Method

# openHelpAnchor(\_:inBook:)

Finds and displays the text at the given anchor location in the given book.

macOS

``` source
@MainActor
func openHelpAnchor(
    _ anchor: NSHelpManager.AnchorName,
    inBook book: NSHelpManager.BookName?
)
```

## Parameters 

`anchor`  

Location of the desired text.

`book`  

Help book containing the anchor. When `nil`, all installed help books are searched.

## Discussion

To open an anchor in your bundle’s localized help book, you could use code similar to the following:

```
NSString *locBookName = [[NSBundle mainBundle] objectForInfoDictionaryKey: @"CFBundleHelpBookName"];
[[NSHelpManager sharedHelpManager] openHelpAnchor:@"anchor1"  inBook:locBookName];
```

This method is a wrapper for `AHRegisterHelpBook` (which is called only once to register the help book specified in the application’s main bundle) and `AHLookupAnchor`.

## See Also

### Displaying Help

func find(String, inBook: NSHelpManager.BookName?)

Performs a search for the specified string in the specified book.

typealias AnchorName

typealias BookName

