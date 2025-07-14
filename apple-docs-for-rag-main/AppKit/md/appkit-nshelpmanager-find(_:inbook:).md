

- AppKit
- NSHelpManager
-  find(\_:inBook:) 

Instance Method

# find(\_:inBook:)

Performs a search for the specified string in the specified book.

macOS

``` source
@MainActor
func find(
    _ query: String,
    inBook book: NSHelpManager.BookName?
)
```

## Parameters 

`query`  

String to search for.

`book`  

Localized help book to search. When `nil`, all installed help books are searched.

## Discussion

To search for a string in your bundle’s localized help book, you could use code similar to the following:

```
NSString *locBookName = [[NSBundle mainBundle] objectForInfoDictionaryKey: @"CFBundleHelpBookName"];
[[NSHelpManager sharedHelpManager] findString:@"Hello"  inBook:locBookName];
```

This is a wrapper for `AHRegisterHelpBook` (which is called only once to register the help book specified in the application’s main bundle) and `AHSearch`.

## See Also

### Displaying Help

func openHelpAnchor(NSHelpManager.AnchorName, inBook: NSHelpManager.BookName?)

Finds and displays the text at the given anchor location in the given book.

typealias AnchorName

typealias BookName

