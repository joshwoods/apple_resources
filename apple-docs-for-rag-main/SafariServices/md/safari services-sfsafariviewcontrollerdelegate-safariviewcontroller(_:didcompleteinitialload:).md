

- Safari Services
- SFSafariViewControllerDelegate
-  safariViewController(\_:didCompleteInitialLoad:) 

Instance Method

# safariViewController(\_:didCompleteInitialLoad:)

Tells the delegate that the initial URL load completed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
optional func safariViewController(
    _ controller: SFSafariViewController,
    didCompleteInitialLoad didLoadSuccessfully: Bool
)
```

## Parameters 

`controller`  

The view controller.

`didLoadSuccessfully`  

true if loading completed successfully; otherwise, false.

## Discussion

This method is invoked when SFSafariViewController completes the loading of the URL that you pass to its initializer. The method is not invoked for any subsequent page loads in the same SFSafariViewController instance.

## See Also

### Working with the View Controller

func safariViewController(SFSafariViewController, activityItemsFor: URL, title: String?) -> [UIActivity]

Tells the delegate that the user tapped an Action button.

func safariViewControllerDidFinish(SFSafariViewController)

Tells the delegate that the user dismissed the view.

func safariViewController(SFSafariViewController, excludedActivityTypesFor: URL, title: String?) -> [UIActivity.ActivityType]

