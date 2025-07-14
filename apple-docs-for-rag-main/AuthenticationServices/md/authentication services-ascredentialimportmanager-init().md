

- Authentication Services
- ASCredentialImportManager
-  init() 

Initializer

# init()

Creates an import manager instance.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
init()
```

## Discussion

Create an instance of this class when the system launches your app with an NSUserActivity of type `ASCredentialExchangeActivityType`, then call importCredentials(token:) to import credentials from the source app.

