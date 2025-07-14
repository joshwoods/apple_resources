

- Foundation
- URL
-  URL.ParseStrategy 

Structure

# URL.ParseStrategy

A parse strategy for creating URLs from formatted strings.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ParseStrategy
```

## Overview

Create an explicit URL.ParseStrategy to parse multiple strings according to the same parse strategy. The following example creates a customized strategy, then applies it to multiple URL candidate strings.

```
let strategy = URL.ParseStrategy(
    scheme: .defaultValue("https"),
    user: .optional,
    password: .optional,
    host: .required,
    port: .optional,
    path: .required,
    query: .required,
    fragment: .optional)
let urlStrings = [
    "example.com?key1=value1", // no scheme or path
    "https://example.com?key2=value2", // no path
    "https://example.com", // no query
    "https://example.com/path?key4=value4", // complete
    "//example.com/path?key5=value5" // complete except for default-able scheme
]
let urls = urlStrings.map { try? strategy.parse($0) } // [nil, nil, nil, Optional(https://example.com/path?key4=value4), Optional(https://example.com/path?key5=value5)]
```

You don’t need to instantiate a parse strategy instance to parse a single string. Instead, use the URL initializer init(_:strategy:), passing in a string to parse and a customized strategy, typically created with one of the static accessors. The following example parses a URL string, with a custom strategy that provides a default value for the port component if the source string doesn’t specify one.

```
let urlString = "https://internal.example.com/path/to/endpoint?key=value"
let url = try? URL(urlString, strategy: .url
    .port(.defaultValue(8080))) // https://internal.example.com:8080/path/to/endpoint?key=value

```

## Topics

### Creating a URL parse strategy

init(scheme: URL.ParseStrategy.ComponentParseStrategy&lt;String>, user: URL.ParseStrategy.ComponentParseStrategy&lt;String>, password: URL.ParseStrategy.ComponentParseStrategy&lt;String>, host: URL.ParseStrategy.ComponentParseStrategy&lt;String>, port: URL.ParseStrategy.ComponentParseStrategy&lt;Int>, path: URL.ParseStrategy.ComponentParseStrategy&lt;String>, query: URL.ParseStrategy.ComponentParseStrategy&lt;String>, fragment: URL.ParseStrategy.ComponentParseStrategy&lt;String>)

Creates a URL parse strategy with the specified component-parsing behaviors.

enum ComponentParseStrategy

The strategy used to parse one component of a URL.

### Customizing strategy behavior

func scheme(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s scheme component in accordance with the provided behavior.

func user(URL.ParseStrategy.ComponentParseStrategy&lt;String>) -> URL.ParseStrategy

Modifies a parse strategy to parse a URL’s user component in accordance with the provided behavior.

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

## Relationships

### Conforms To

- Copyable
- CustomConsumingRegexComponent
- Decodable
- Encodable
- Equatable
- Hashable
- ParseStrategy
- RegexComponent
- Sendable

