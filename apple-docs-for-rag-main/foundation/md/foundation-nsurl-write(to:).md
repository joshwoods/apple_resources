

- Foundation
- NSURL
-  write(to:) 

Instance Method

# write(to:)

Writes the URL to the specified pasteboard.

macOS 10.0+

``` source
func write(to pasteBoard: NSPasteboard)
```

## Parameters 

`pasteBoard`  

The target pasteboard.

## Discussion

You must declare an `NSURLPboardType` data type for the pasteboard before invoking this method. Otherwise, the method returns without doing anything.

## See Also

### Related Documentation

func declareTypes(_ newTypes: [NSPasteboard.PasteboardType], owner newOwner: Any?) -> Int

Prepares the receiver for a change in its contents by declaring the new types of data it will contain and a new owner.

### Working with Pasteboards

init?(fromPasteboard: NSPasteboard)

Reads an NSURL object off of the specified pasteboard.

