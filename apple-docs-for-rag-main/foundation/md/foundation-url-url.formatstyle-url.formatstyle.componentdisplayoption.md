

- Foundation
- URL
- URL.FormatStyle
-  URL.FormatStyle.ComponentDisplayOption 

Structure

# URL.FormatStyle.ComponentDisplayOption

A type that indicates whether a formatted URL should include a component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ComponentDisplayOption
```

## Topics

### Display options

static var always: URL.FormatStyle.ComponentDisplayOption

A display option that always displays the component.

static var never: URL.FormatStyle.ComponentDisplayOption

A display option that never displays the component.

static var omitIfHTTPFamily: URL.FormatStyle.ComponentDisplayOption

A display option that omits the component if the URL scheme is any flavor of HTTP.

static func displayWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.ComponentDisplayOption

Returns a display option that displays the component when a specified component meets the specified requirements.

static func omitWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.ComponentDisplayOption

Returns a display option that omits the component when a specified component meets the specified requirements.

enum Component

An enumeration of the components of a URL, for use in creating format style options that depend on a component’s value.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a URL format style

init(scheme: URL.FormatStyle.ComponentDisplayOption, user: URL.FormatStyle.ComponentDisplayOption, password: URL.FormatStyle.ComponentDisplayOption, host: URL.FormatStyle.HostDisplayOption, port: URL.FormatStyle.ComponentDisplayOption, path: URL.FormatStyle.ComponentDisplayOption, query: URL.FormatStyle.ComponentDisplayOption, fragment: URL.FormatStyle.ComponentDisplayOption)

Creates a URL format style with the given display options.

struct HostDisplayOption

A type that indicates whether a formatted URL should include the host component.

