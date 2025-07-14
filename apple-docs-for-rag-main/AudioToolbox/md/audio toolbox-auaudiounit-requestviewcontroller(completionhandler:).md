

- Audio Toolbox
- AUAudioUnit
-  requestViewController(completionHandler:) 

Instance Method

# requestViewController(completionHandler:)

Requests an audio unit’s custom view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

**macOS**

``` source
func requestViewController(completionHandler: @escaping (NSViewController?) -> Void)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func requestViewController(completionHandler: @escaping (UIViewController?) -> Void)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func requestViewController() async -> UIViewController?
```

**macOS**

``` source
func requestViewController() async -> NSViewController?
```

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

The completion handler is called on a thread or dispatch queue internal to the audio unit’s implementation. If the audio unit does not implement a custom view controller, it returns `nil`. If it has a custom view controller, it instantiates the view controller and returns it. The custom view controller must be a subclass of AUViewController.

