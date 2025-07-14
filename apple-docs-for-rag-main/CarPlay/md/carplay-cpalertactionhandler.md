

- CarPlay
-  CPAlertActionHandler 

Type Alias

# CPAlertActionHandler

The declaration for an alert action handler.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+

``` source
typealias CPAlertActionHandler = (CPAlertAction) -> Void
```

## Parameters 

`action`  

The alert action that invoked the block.

## See Also

### Getting the Action Handler

var handler: CPAlertActionHandler

The closure that CarPlay invokes after the user taps the action button.

