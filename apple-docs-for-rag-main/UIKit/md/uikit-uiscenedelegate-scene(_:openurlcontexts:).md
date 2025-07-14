

- UIKit
- UISceneDelegate
-  scene(\_:openURLContexts:) 

Instance Method

# scene(\_:openURLContexts:)

Asks the delegate to open one or more URLs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    openURLContexts URLContexts: Set
)
```

## Parameters 

`scene`  

The scene that UIKit asks to open the URL.

`URLContexts`  

One or more UIOpenURLContext objects. Each object contains one URL to open and any additional information needed to open that URL.

## Mentioned in 

Collaborating and sharing copies of your data

