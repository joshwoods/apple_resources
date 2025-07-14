

- AppKit
- NSOpenSavePanelDelegate
-  panel(\_:shouldEnable:) 

Instance Method

# panel(\_:shouldEnable:)

Asks the delegate whether the specified URL should be enabled in the Open panel.

macOS 10.6+

``` source
@MainActor
optional func panel(
    _ sender: Any,
    shouldEnable url: URL
) -> Bool
```

## Parameters 

`sender`  

The panel that asks whether the URL should be enabled.

`url`  

The URL for you to check.

## Return Value

true if you want the panel to display the item at the specifed URL as enabled, or false to display it as disabled.

## Discussion

Save panels do not call this method; they always disable URLs. Implementations of this method should be fast to avoid stalling the user interface. Use panel(_:validate:) instead if processing will take a long time.

## See Also

### Related Documentation

Sheet Programming Topics

### Validating the Panel Content

func panel(Any, validate: URL) throws

Asks the delegate to validate the URL for a file that the user selected.

