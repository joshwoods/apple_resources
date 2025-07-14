

- Foundation
- URL
- URL.FormatStyle
- URL.FormatStyle.ComponentDisplayOption
-  omitWhen(\_:matches:) 

Type Method

# omitWhen(\_:matches:)

Returns a display option that omits the component when a specified component meets the specified requirements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func omitWhen(
    _ component: URL.FormatStyle.Component,
    matches requirements: Set
) -> URL.FormatStyle.ComponentDisplayOption
```

## Parameters 

`component`  

A component to compare. This may or may not be the component the strategy modifies. For example, a display option for the password might match against known values for the user.

`requirements`  

A set of string values to match against. Matching any member of the set informs the format style to omit the component.

## Return Value

A display option that omits the component when a specified component meets the specified requirements.

## See Also

### Display options

static var always: URL.FormatStyle.ComponentDisplayOption

A display option that always displays the component.

static var never: URL.FormatStyle.ComponentDisplayOption

A display option that never displays the component.

static var omitIfHTTPFamily: URL.FormatStyle.ComponentDisplayOption

A display option that omits the component if the URL scheme is any flavor of HTTP.

static func displayWhen(URL.FormatStyle.Component, matches: Set&lt;String>) -> URL.FormatStyle.ComponentDisplayOption

Returns a display option that displays the component when a specified component meets the specified requirements.

enum Component

An enumeration of the components of a URL, for use in creating format style options that depend on a component’s value.

