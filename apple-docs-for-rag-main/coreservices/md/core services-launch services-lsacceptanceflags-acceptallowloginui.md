

- Core Services
- Launch Services
- LSAcceptanceFlags
-  acceptAllowLoginUI 

Type Property

# acceptAllowLoginUI

Requests that the user interface to log in be presented.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var acceptAllowLoginUI: LSAcceptanceFlags { get }
```

## Discussion

If `LSCanRefAcceptItem` or `LSCanURLAcceptURL` is called during a drag-and-drop operation, showing a server login dialog would be an inappropriate user experience. If the target designated in the function call is an alias to an application, Launch Services needs to resolve the alias to ascertain what file types the application can open.

If the application is on a server that needs to be authenticated, Launch Services will fail to resolve the alias to avoid having to present the login interface.To override this default behavior by allowing the server login interface, set the `kLSAcceptAllowLoginUI` flag.

