

- AppKit
- NSPasteboardItem
-  setDataProvider(\_:forTypes:) 

Instance Method

# setDataProvider(\_:forTypes:)

Sets the data provider for the specified types.

macOS 10.6+

``` source
func setDataProvider(
    _ dataProvider: any NSPasteboardItemDataProvider,
    forTypes types: [NSPasteboard.PasteboardType]
) -> Bool
```

## Parameters 

`dataProvider`  

A pasteboard data provider.

`types`  

An array of strings indicating the UTIs for the data representations `dataProvider` may provide.

## Return Value

true if the data provider was set successfully, otherwise false.

## Discussion

This method registers the data provider to be messaged to provide the data for any of the specified types when requested.

