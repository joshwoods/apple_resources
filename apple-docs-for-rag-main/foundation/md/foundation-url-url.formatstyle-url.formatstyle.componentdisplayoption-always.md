

- Foundation
- URL
- URL.FormatStyle
- URL.FormatStyle.ComponentDisplayOption
-  always 

Type Property

# always

A display option that always displays the component.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var always: URL.FormatStyle.ComponentDisplayOption { get }
```

## See Also

### Display options

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

