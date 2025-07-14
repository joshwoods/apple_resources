

- AppKit
- NSSpellChecker
-  menu(for:string:options:atLocation:in:) 

Instance Method

# menu(for:string:options:atLocation:in:)

Provides a menu containing contextual menu items suitable for certain kinds of detected results.

macOS 10.6+

``` source
func menu(
    for result: NSTextCheckingResult,
    string checkedString: String,
    options: [NSSpellChecker.OptionKey : Any]? = nil,
    atLocation location: NSPoint,
    in view: NSView
) -> NSMenu?
```

## Parameters 

`result`  

The NSTextCheckingResult instance for the checked string.

`checkedString`  

The string that has been checked.

`options`  

The options dictionary allows clients to pass in information associated with the document. See `Spell Checking Option Dictionary Keys` for possible key-value pairs.

`location`  

The location, in the view’s coordinate system, to display the menu.

`view`  

The view object over which to display the contextual menu.

## Return Value

A menu suitable for displaying as a contextual menu, or adding to another contextual menu as a submenu.

## See Also

### Data Detector Interaction

struct OptionKey

The constants are optional keys that can be used in the options dictionary parameter of the check(_:range:types:options:inSpellDocumentWithTag:orthography:wordCount:), requestChecking(of:range:types:options:inSpellDocumentWithTag:completionHandler:), and menu(for:string:options:atLocation:in:) methods.

