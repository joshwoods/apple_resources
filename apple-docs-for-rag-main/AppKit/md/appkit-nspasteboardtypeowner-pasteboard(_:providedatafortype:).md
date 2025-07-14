

- AppKit
- NSPasteboardTypeOwner
-  pasteboard(\_:provideDataForType:) 

Instance Method

# pasteboard(\_:provideDataForType:)

Requests that the object provide data for the data type to the pasteboard.

macOS

``` source
func pasteboard(
    _ sender: NSPasteboard,
    provideDataForType type: NSPasteboard.PasteboardType
)
```

**Required**

## Parameters 

`sender`  

The pasteboard requesting data.

`type`  

The data type.

