

- Foundation
- URL
- URL.ParseStrategy
-  init(scheme:user:password:host:port:path:query:fragment:) 

Initializer

# init(scheme:user:password:host:port:path:query:fragment:)

Creates a URL parse strategy with the specified component-parsing behaviors.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    scheme: URL.ParseStrategy.ComponentParseStrategy = .required,
    user: URL.ParseStrategy.ComponentParseStrategy = .optional,
    password: URL.ParseStrategy.ComponentParseStrategy = .optional,
    host: URL.ParseStrategy.ComponentParseStrategy = .required,
    port: URL.ParseStrategy.ComponentParseStrategy = .optional,
    path: URL.ParseStrategy.ComponentParseStrategy = .optional,
    query: URL.ParseStrategy.ComponentParseStrategy = .optional,
    fragment: URL.ParseStrategy.ComponentParseStrategy = .optional
)
```

## Parameters 

`scheme`  

A strategy for parsing the scheme component.

`user`  

A strategy for parsing the user component.

`password`  

A strategy for parsing the password component.

`host`  

A strategy for parsing the host component.

`port`  

A strategy for parsing the port component.

`path`  

A strategy for parsing the path component.

`query`  

A strategy for parsing the query component.

`fragment`  

A strategy for parsing the fragment component.

## See Also

### Creating a URL parse strategy

enum ComponentParseStrategy

The strategy used to parse one component of a URL.

