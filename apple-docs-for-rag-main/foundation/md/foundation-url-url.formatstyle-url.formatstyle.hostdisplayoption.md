

- Foundation
- URL
- URL.FormatStyle
-  URL.FormatStyle.HostDisplayOption 

Structure

# URL.FormatStyle.HostDisplayOption

A type that indicates whether a formatted URL should include the host component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct HostDisplayOption
```

## Topics

### Display options

static var always: URL.FormatStyle.HostDisplayOption

A display option that always displays the host component.

static var never: URL.FormatStyle.HostDisplayOption

A display option that never displays the host component.

static var omitIfHTTPFamily: URL.FormatStyle.HostDisplayOption

A display option that omits the host component if the URL scheme is HTTP or HTTPS.

static func displayWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.HostDisplayOption

Returns a display option that displays the host component when a specified component matches against a set of requirement values.

static func omitWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.HostDisplayOption

Returns a display option that displays the host component when a specified component matches against a set of requirement values.

static func omitSpecificSubdomains(Set&lt;String>, includeMultiLevelSubdomains: Bool) -> URL.FormatStyle.HostDisplayOption

Returns a display option that omits the host component if it matches a set of subdomains.

static func omitSpecificSubdomains(Set&lt;String>, includeMultiLevelSubdomains: Bool, when: URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.HostDisplayOption

Returns a display option that omits the host component if it matches a set of subdomains and a specified component matches a set of requirements.

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

struct ComponentDisplayOption

A type that indicates whether a formatted URL should include a component.

