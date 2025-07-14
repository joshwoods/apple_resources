

- Objective-C Runtime
- NSObject
-  authorizationViewDidHide(\_:) 

Instance Method

# authorizationViewDidHide(\_:)

Sent to the delegate to indicate that the view’s visibility has changed.

macOS 10.3+

``` source
func authorizationViewDidHide(_ view: SFAuthorizationView!)
```

## Discussion

This delegate method, if present, is called whenever the isHidden method is called to show or hide the view.

