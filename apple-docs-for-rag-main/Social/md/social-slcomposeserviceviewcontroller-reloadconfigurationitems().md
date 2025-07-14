

- Social
- SLComposeServiceViewController
-  reloadConfigurationItems() 

Instance Method

# reloadConfigurationItems()

Reloads the list of configuration items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
@MainActor
func reloadConfigurationItems()
```

## Discussion

In general, a subclass doesn’t need to call this method, unless it determines its configuration items in a deferred way, such as in presentationAnimationDidFinish(). In particular, you don’t need to call this method after you change a configuration item property, because the `SLComposeServiceViewController` base class automatically detects and responds to such changes.

## See Also

### Configuring the Post Details

func configurationItems() -> [Any]!

Returns configuration items to display in the compose view.

class SLComposeSheetConfigurationItem

An object that provides additional configuration details to use when configuring a composition interface.

