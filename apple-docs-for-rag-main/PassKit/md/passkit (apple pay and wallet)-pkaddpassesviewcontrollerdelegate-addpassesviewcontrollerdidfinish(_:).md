

- PassKit (Apple Pay and Wallet)
- PKAddPassesViewControllerDelegate
-  addPassesViewControllerDidFinish(\_:) 

Instance Method

# addPassesViewControllerDidFinish(\_:)

Sent to the delegate after the add-passes view controller has finished.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func addPassesViewControllerDidFinish(_ controller: PKAddPassesViewController)
```

## Discussion

When this optional method is implemented, the delegate is responsible for dismissing the view controller in `controller`.

## See Also

### Related Documentation

Wallet Developer Guide

