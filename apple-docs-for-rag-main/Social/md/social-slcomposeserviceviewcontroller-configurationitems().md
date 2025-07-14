

- Social
- SLComposeServiceViewController
-  configurationItems() 

Instance Method

# configurationItems()

Returns configuration items to display in the compose view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
@MainActor
func configurationItems() -> [Any]!
```

## Return Value

An array of SLComposeSheetConfigurationItem objects, or `nil` if no configuration items need to be displayed.

## Discussion

Implement this method if you need to display configuration items, such as an account picker or privacy indicator, in your compose view.

## See Also

### Configuring the Post Details

class SLComposeSheetConfigurationItem

An object that provides additional configuration details to use when configuring a composition interface.

func reloadConfigurationItems()

Reloads the list of configuration items.

