

- Core Services
- Apple Events
- Launch Apple Event Constants
-  keyAELaunchedAsServiceItem 

Global Variable

# keyAELaunchedAsServiceItem

Mac Catalyst 13.0+macOS 10.5+

``` source
var keyAELaunchedAsServiceItem: AEKeyword { get }
```

## Discussion

If present in a `kAEOpenApplication` event, the receiving application was launched as a service item and should only perform actions suitable to that environment—for example, it probably shouldn't open an untitled document.

