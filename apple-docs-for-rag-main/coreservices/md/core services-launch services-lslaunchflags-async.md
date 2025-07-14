

- Core Services
- Launch Services
- LSLaunchFlags
-  async 

Type Property

# async

Requests that the application be launched asynchronously.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var async: LSLaunchFlags { get }
```

## Discussion

The Launch Services function launching it returns control immediately without waiting for it to complete its launch sequence (indicated visually to the user when the application’s icon stops “bouncing” in the Dock).

