

- Safari Services
- SFSafariViewControllerDelegate
-  safariViewController(\_:activityItemsFor:title:) 

Instance Method

# safariViewController(\_:activityItemsFor:title:)

Tells the delegate that the user tapped an Action button.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
optional func safariViewController(
    _ controller: SFSafariViewController,
    activityItemsFor URL: URL,
    title: String?
) -> [UIActivity]
```

## Parameters 

`controller`  

The view controller.

`URL`  

The URL of the web page that was active when the Action button was tapped.

`title`  

The title of the web page.

## Return Value

An array of application-specific services you have chosen to include in the UIActivityViewController object.

## Discussion

The view controller calls this method when the view is about to show an activity view controller. Your delegate can provide unique, application-specific services (such as a social media service) to be included with the system-provided sharing services. See UIActivity.

## See Also

### Working with the View Controller

func safariViewController(SFSafariViewController, didCompleteInitialLoad: Bool)

Tells the delegate that the initial URL load completed.

func safariViewControllerDidFinish(SFSafariViewController)

Tells the delegate that the user dismissed the view.

func safariViewController(SFSafariViewController, excludedActivityTypesFor: URL, title: String?) -> [UIActivity.ActivityType]

