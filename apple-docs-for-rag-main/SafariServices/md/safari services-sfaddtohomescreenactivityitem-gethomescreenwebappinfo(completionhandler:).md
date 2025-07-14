

- Safari Services
- SFAddToHomeScreenActivityItem
-  getHomeScreenWebAppInfo(completionHandler:) 

Instance Method

# getHomeScreenWebAppInfo(completionHandler:)

Provides information about a web app to the system.

iOS 18.2+iPadOS 18.2+visionOS 2.2+

``` source
optional func getHomeScreenWebAppInfo(completionHandler: @escaping (SFAddToHomeScreenInfo?) -> Void)
```

``` source
optional func homeScreenWebAppInfo() async -> SFAddToHomeScreenInfo?
```

## Parameters 

`completionHandler`  

A closure that you call to supply the web app’s information to the system.

## Overview

Add information about the web app to a SFAddToHomeScreenInfo object that you create, and pass it to the completion handler.

The system only calls this method in browser apps that include an alternative browser engine. If you implement this method, then the system doesn’t call your implementation of getWebAppManifest(completionHandler:).

## See Also

### Providing information about a web app to the system

class SFAddToHomeScreenInfo

A class that provides information about a web app that someone adds to their Home Screen.

func getWebAppManifest(completionHandler: (BEWebAppManifest?) -> Void)

Provides the web app’s manifest to the system, if the bookmark represents a web app.

