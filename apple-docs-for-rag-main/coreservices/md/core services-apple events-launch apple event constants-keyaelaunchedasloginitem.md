

- Core Services
- Apple Events
- Launch Apple Event Constants
-  keyAELaunchedAsLogInItem 

Global Variable

# keyAELaunchedAsLogInItem

If present in a `kAEOpenApplication` event, the receiving application was launched as a login item and should only perform actions suitable to that environment—for example, it probably shouldn't open an untitled document.

Mac Catalyst 13.0+macOS 10.5+

``` source
var keyAELaunchedAsLogInItem: AEKeyword { get }
```

