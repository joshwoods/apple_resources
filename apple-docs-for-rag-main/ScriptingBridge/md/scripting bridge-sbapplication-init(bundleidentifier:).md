

- Scripting Bridge
- SBApplication
-  init(bundleIdentifier:) 

Initializer

# init(bundleIdentifier:)

Returns an instance of an `SBApplication` subclass that represents the target application identified by the given bundle identifier.

Mac Catalyst 13.0+macOS 10.5+

``` source
init?(bundleIdentifier ident: String)
```

## Parameters 

`ident`  

A bundle identifier specifying an application that is OSA-compliant.

## Return Value

An initialized shared instance of an `SBApplication` subclass that represents a target application with the bundle identifier of `ident`. Returns `nil` if no such application can be found or if the application does not have a scripting interface.

## Discussion

If you must initialize an `SBApplication` object explictly, you should use this initializer if possible; unlike init(processIdentifier:) and init(url:), this method is not dependent on changeable factors such as the target application’s path or process ID. Even so, you should rarely have to initialize an `SBApplication` object yourself; instead, you should initialize an application-specific subclass such as `iTunesApplication`.

Note that this method does not check whether an application with the given bundle identifier actually exists.

## See Also

### Initializing a Scriptable Application Object

init?(processIdentifier: pid_t)

Returns an instance of an `SBApplication` subclass that represents the target application identified by the given process identifier.

init?(url: URL)

Returns an instance of an `SBApplication` subclass that represents the target application identified by the given URL.

