

- UIKit
- UISearchDisplayDelegate
-  searchDisplayControllerDidBeginSearch(\_:) Deprecated

Instance Method

# searchDisplayControllerDidBeginSearch(\_:)

Tells the delegate that the controller has started searching.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
optional func searchDisplayControllerDidBeginSearch(_ controller: UISearchDisplayController)
```

## Parameters 

`controller`  

The search display controller for which the receiver is the delegate.

## See Also

### Responding to search state change

func searchDisplayControllerWillBeginSearch(UISearchDisplayController)

Tells the delegate that the controller is about to begin searching.

Deprecated

func searchDisplayControllerWillEndSearch(UISearchDisplayController)

Tells the delegate that the controller is about to end searching.

Deprecated

func searchDisplayControllerDidEndSearch(UISearchDisplayController)

Tells the delegate that the controller has finished searching.

Deprecated

