

- Safari Services
- SFSafariExtensionHandling
-  contextMenuItemSelected(withCommand:in:userInfo:) 

Instance Method

# contextMenuItemSelected(withCommand:in:userInfo:)

A method the system calls when a user selects one of the app extension’s context menu items.

macOS 10.12+

``` source
optional func contextMenuItemSelected(
    withCommand command: String,
    in page: SFSafariPage,
    userInfo: [String : Any]? = nil
)
```

## Parameters 

`command`  

The command that is associated with the selected context menu item specified in `Info.plist`.

`page`  

The page where the context menu item was selected.

`userInfo`  

Optional message content. If specified, the dictionary’s value objects conform to the W3C standard for safe passing of structured data, such as Boolean objects, numeric values, strings, and arrays.

## Mentioned in 

Adjusting settings for contextual menu items

## See Also

### Responding to Context Menu Selections

func validateContextMenuItem(withCommand: String, in: SFSafariPage, userInfo: [String : Any]?, validationHandler: (Bool, String?) -> Void)

Validates whether a particular contextual menu item should be displayed.

