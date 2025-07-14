

- WebKit
- WKUserContentController
-  removeAllUserScripts() 

Instance Method

# removeAllUserScripts()

Removes all user scripts from the web view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func removeAllUserScripts()
```

## See Also

### Adding and Removing Custom Scripts

func addUserScript(WKUserScript)

Injects the specified script into the webpage’s content.

var userScripts: [WKUserScript]

The user scripts associated with the user content controller.

