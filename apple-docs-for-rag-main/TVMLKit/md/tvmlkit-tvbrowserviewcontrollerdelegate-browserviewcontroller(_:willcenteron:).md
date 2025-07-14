

- TVMLKit
- TVBrowserViewControllerDelegate
-  browserViewController(\_:willCenterOn:) 

Instance Method

# browserViewController(\_:willCenterOn:)

Tells the delegate when the specified view element is to be centered on the page.

tvOS 13.0+

``` source
optional func browserViewController(
    _ browserViewController: TVBrowserViewController,
    willCenterOn viewElement: TVViewElement
)
```

## See Also

### Managing Focus

func browserViewController(TVBrowserViewController, didCenterOn: TVViewElement)

Tells the delegate how to respond when the specified view element completes the transition to becoming centered upon.

