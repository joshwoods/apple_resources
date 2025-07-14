

- AppKit
- NSViewControllerPresentationAnimator
-  animateDismissal(of:from:) 

Instance Method

# animateDismissal(of:from:)

Called when a previously-presented view controller is about to be dismissed.

macOS 10.10+

``` source
@MainActor
func animateDismissal(
    of viewController: NSViewController,
    from fromViewController: NSViewController
)
```

**Required**

## Parameters 

`viewController`  

The view controller that is being dismissed.

`fromViewController`  

The view controller that is the parent of the one in the `viewController` parameter.

## Discussion

To add custom view controller dismissal animation, Implement it in this method.

## See Also

### Animating Presentation and Dismissal of View Controllers

func animatePresentation(of: NSViewController, from: NSViewController)

Called when the specified view controller is about to be presented.

**Required**

