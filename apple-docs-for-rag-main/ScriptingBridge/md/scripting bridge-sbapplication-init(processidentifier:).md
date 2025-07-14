

- Scripting Bridge
- SBApplication
-  init(processIdentifier:) 

Initializer

# init(processIdentifier:)

Returns an instance of an `SBApplication` subclass that represents the target application identified by the given process identifier.

Mac Catalyst 13.0+macOS 10.5+

``` source
init?(processIdentifier pid: pid_t)
```

## Parameters 

`pid`  

A BSD process ID specifying an application that is OSA-compliant. Often you can get the process ID of a process using the processIdentifier method of `NSTask`.

## Return Value

An initialized `SBApplication` that you can use to communicate with the target application specified by the process ID. Returns `nil` if no such application can be found or if the application does not have a scripting interface.

## Discussion

You should avoid using this method unless you know nothing about an external application but its PID. In most cases, it is better to use init(bundleIdentifier:), which will dynamically locate the external application’s path at runtime, or init(url:), which is not dependent on the external application being open at the time the method is called.

## See Also

### Initializing a Scriptable Application Object

init?(bundleIdentifier: String)

Returns an instance of an `SBApplication` subclass that represents the target application identified by the given bundle identifier.

init?(url: URL)

Returns an instance of an `SBApplication` subclass that represents the target application identified by the given URL.

