

- AppKit
- NSViewControllerPresentationAnimator
-  animatePresentation(of:from:) 

Instance Method

# animatePresentation(of:from:)

Called when the specified view controller is about to be presented.

macOS 10.10+

``` source
@MainActor
func animatePresentation(
    of viewController: NSViewController,
    from fromViewController: NSViewController
)
```

**Required**

## Parameters 

`viewController`  

The view controller that is being presented in place of the one in the `fromViewController` parameter.

`fromViewController`  

The view controller that is the parent of the one in the `viewController` parameter.

## Discussion

To add custom presentation animation, Implement it in this method.

## See Also

### Animating Presentation and Dismissal of View Controllers

func animateDismissal(of: NSViewController, from: NSViewController)

Called when a previously-presented view controller is about to be dismissed.

**Required**

