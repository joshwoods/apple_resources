

- Social
- SLComposeServiceViewController
-  pushConfigurationViewController(\_:) 

Instance Method

# pushConfigurationViewController(\_:)

Presents a configuration view controller that lets the user configure the post.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
@MainActor
func pushConfigurationViewController(_ viewController: UIViewController!)
```

## Parameters 

`viewController`  

The view controller that manages the type of configuration the user selected.

## Discussion

Typically, this method is called in the tap handler for a configuration item. A user selects a configuration item from the list displayed in the compose view and the associated configuration view controller is displayed. Only one configuration view controller can be visible at a time.

Note that your custom configuration view controller should set its preferredContentSize property to an appropriate value. `SLComposeServiceViewController` observes changes to the preferredContentSize property and animates view size changes if necessary.

## See Also

### Presenting the View Controller

func popConfigurationViewController()

Dismisses the current configuration view controller.

