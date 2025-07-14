

- WebKit
- WKUserContentController
-  addUserScript(\_:) 

Instance Method

# addUserScript(\_:)

Injects the specified script into the webpage’s content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func addUserScript(_ userScript: WKUserScript)
```

## Parameters 

`userScript`  

The user script to add to the web view’s current page.

## See Also

### Adding and Removing Custom Scripts

func removeAllUserScripts()

Removes all user scripts from the web view.

var userScripts: [WKUserScript]

The user scripts associated with the user content controller.

