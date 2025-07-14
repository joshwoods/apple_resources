

- Safari Services
- SFSafariViewControllerDelegate
-  safariViewController(\_:excludedActivityTypesFor:title:) 

Instance Method

# safariViewController(\_:excludedActivityTypesFor:title:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func safariViewController(
    _ controller: SFSafariViewController,
    excludedActivityTypesFor URL: URL,
    title: String?
) -> [UIActivity.ActivityType]
```

## See Also

### Working with the View Controller

func safariViewController(SFSafariViewController, didCompleteInitialLoad: Bool)

Tells the delegate that the initial URL load completed.

func safariViewController(SFSafariViewController, activityItemsFor: URL, title: String?) -> [UIActivity]

Tells the delegate that the user tapped an Action button.

func safariViewControllerDidFinish(SFSafariViewController)

Tells the delegate that the user dismissed the view.

