

- Security
-  kAuthorizationRightExecute 

Global Variable

# kAuthorizationRightExecute

The type for an authorization item requesting the right to execute with privileges.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAuthorizationRightExecute: String { get }
```

## Discussion

In addition to this right, you should obtain whatever rights the tool needs to perform its operation on your behalf. The AuthorizationItem should contain the full path of the tool you wish to execute in the `value` and `valueLength` fields. In the future we will limit the right to only execute the requested path, and we will display this information to the user.

