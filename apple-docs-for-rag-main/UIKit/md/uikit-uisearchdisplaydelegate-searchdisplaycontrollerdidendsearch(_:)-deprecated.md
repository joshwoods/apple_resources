

- UIKit
- UISearchDisplayDelegate
-  searchDisplayControllerDidEndSearch(\_:) Deprecated

Instance Method

# searchDisplayControllerDidEndSearch(\_:)

Tells the delegate that the controller has finished searching.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayControllerDidEndSearch(_ controller: UISearchDisplayController)
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

## See Also

### Responding to search state change

func searchDisplayControllerWillBeginSearch(UISearchDisplayController)

Tells the delegate that the controller is about to begin searching.

Deprecated

func searchDisplayControllerDidBeginSearch(UISearchDisplayController)

Tells the delegate that the controller has started searching.

Deprecated

func searchDisplayControllerWillEndSearch(UISearchDisplayController)

Tells the delegate that the controller is about to end searching.

Deprecated

