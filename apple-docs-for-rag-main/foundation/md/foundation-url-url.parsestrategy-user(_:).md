

- Foundation
- URL
- URL.ParseStrategy
-  user(\_:) 

Instance Method

# user(\_:)

Modifies a parse strategy to parse a URL’s user component in accordance with the provided behavior.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func user(_ strategy: URL.ParseStrategy.ComponentParseStrategy = .optional) -> URL.ParseStrategy
```

## Parameters 

`strategy`  

A strategy for parsing the usr component.

## Return Value

A modified URL.ParseStrategy that incorporates the specified behavior.

## See Also

### Customizing strategy behavior

func scheme(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s scheme component in accordance with the provided behavior.

func password(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s password component in accordance with the provided behavior.

func host(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s host component in accordance with the provided behavior.

func port(URL.ParseStrategy.ComponentParseStrategy&lt;Int>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s port component in accordance with the provided behavior.

func path(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s path component in accordance with the provided behavior.

func query(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s query component in accordance with the provided behavior.

func fragment(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s fragment component in accordance with the provided behavior.

enum ComponentParseStrategy

The strategy used to parse one component of a URL.

