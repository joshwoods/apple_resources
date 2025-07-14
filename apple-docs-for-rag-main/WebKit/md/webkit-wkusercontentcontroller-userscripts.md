

- WebKit
- WKUserContentController
-  userScripts 

Instance Property

# userScripts

The user scripts associated with the user content controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var userScripts: [WKUserScript] { get }
```

## See Also

### Adding and Removing Custom Scripts

func addUserScript(WKUserScript)

Injects the specified script into the webpage’s content.

func removeAllUserScripts()

Removes all user scripts from the web view.

