

- Foundation
- NSXPCListener
-  init(machServiceName:) 

Initializer

# init(machServiceName:)

Initializes a listener in a LaunchAgent or LaunchDaemon which has a name advertised in a `launchd.plist` file.

macOS 10.8+

``` source
init(machServiceName name: String)
```

## Discussion

For example, you might use this in an agent launched by launchd with a `launchd.plist` contained in `~/Library/LaunchAgents`, or a daemon launched by launchd with a `launchd.plist` contained in `/Library/LaunchDaemons`.

