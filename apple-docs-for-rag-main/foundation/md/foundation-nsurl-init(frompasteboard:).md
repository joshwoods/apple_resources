

- Foundation
- NSURL
-  init(fromPasteboard:) 

Initializer

# init(fromPasteboard:)

Reads an NSURL object off of the specified pasteboard.

macOS 10.0+

``` source
init?(fromPasteboard pasteBoard: NSPasteboard)
```

``` source
init?(from pasteBoard: NSPasteboard)
```

## Parameters 

`pasteBoard`  

The target pasteboard.

## Return Value

A `NSURL` object, or `nil` if the pasteboard does not contain `NSURLPboardType` data.

## See Also

### Working with Pasteboards

func write(to: NSPasteboard)

Writes the URL to the specified pasteboard.

