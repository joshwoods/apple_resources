

- Safari Services
- SFSafariViewControllerDelegate
-  safariViewControllerDidFinish(\_:) 

Instance Method

# safariViewControllerDidFinish(\_:)

Tells the delegate that the user dismissed the view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
optional func safariViewControllerDidFinish(_ controller: SFSafariViewController)
```

## Parameters 

`controller`  

The view controller.

## Discussion

You can perform any necessary cleanup here. The view controller is dismissed afterwards.

## See Also

### Working with the View Controller

func safariViewController(SFSafariViewController, didCompleteInitialLoad: Bool)

Tells the delegate that the initial URL load completed.

func safariViewController(SFSafariViewController, activityItemsFor: URL, title: String?) -> [UIActivity]

Tells the delegate that the user tapped an Action button.

func safariViewController(SFSafariViewController, excludedActivityTypesFor: URL, title: String?) -> [UIActivity.ActivityType]

