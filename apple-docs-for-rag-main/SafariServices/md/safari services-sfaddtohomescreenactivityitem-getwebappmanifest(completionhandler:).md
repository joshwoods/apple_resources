

- Safari Services
- SFAddToHomeScreenActivityItem
-  getWebAppManifest(completionHandler:) 

Instance Method

# getWebAppManifest(completionHandler:)

Provides the web app’s manifest to the system, if the bookmark represents a web app.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+visionOS 1.2+

``` source
optional func getWebAppManifest(completionHandler: @escaping (BEWebAppManifest?) -> Void)
```

``` source
optional func webAppManifest() async -> BEWebAppManifest?
```

## Parameters 

`completionHandler`  

A closure that you call to supply the web app manifest to the system.

## Discussion

The system only calls this method in browser apps that include an alternative browser engine.

## See Also

### Providing information about a web app to the system

func getHomeScreenWebAppInfo(completionHandler: (SFAddToHomeScreenInfo?) -> Void)

Provides information about a web app to the system.

class SFAddToHomeScreenInfo

A class that provides information about a web app that someone adds to their Home Screen.

