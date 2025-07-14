

- TVMLKit
- TVBrowserViewControllerDelegate
-  browserViewController(\_:didCenterOn:) 

Instance Method

# browserViewController(\_:didCenterOn:)

Tells the delegate how to respond when the specified view element completes the transition to becoming centered upon.

tvOS 13.0+

``` source
optional func browserViewController(
    _ browserViewController: TVBrowserViewController,
    didCenterOn viewElement: TVViewElement
)
```

## See Also

### Managing Focus

func browserViewController(TVBrowserViewController, willCenterOn: TVViewElement)

Tells the delegate when the specified view element is to be centered on the page.

