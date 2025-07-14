

- Foundation
- NSExtensionContext
-  loadBroadcastingApplicationInfo(completion:) 

Instance Method

# loadBroadcastingApplicationInfo(completion:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 11.0+tvOS 9.0+visionOS 1.0+

**macOS**

``` source
func loadBroadcastingApplicationInfo(completion handler: @escaping (String, String, NSImage?) -> Void)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func loadBroadcastingApplicationInfo(completion handler: @escaping (String, String, UIImage?) -> Void)
```

**macOS**

``` source
func loadBroadcastingApplicationInfo() async -> (String, String, NSImage?)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func loadBroadcastingApplicationInfo() async -> (String, String, UIImage?)
```

## Discussion

## See Also

### Supporting broadcasting

func completeRequest(withBroadcast: URL, setupInfo: [String : any NSCoding &amp; NSObjectProtocol]?)

