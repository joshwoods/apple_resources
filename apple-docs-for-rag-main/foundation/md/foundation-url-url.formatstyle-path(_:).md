

- Foundation
- URL
- URL.FormatStyle
-  path(\_:) 

Instance Method

# path(\_:)

Modifies a format style to display a URL’s path component in accordance with the provided option.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func path(_ strategy: URL.FormatStyle.ComponentDisplayOption = .always) -> URL.FormatStyle
```

## Parameters 

`strategy`  

A component display option that indicates when, if ever, to display the path component.

## Return Value

A modified URL.FormatStyle that incorporates the specified behavior.

## See Also

### Customizing style behavior

func scheme(URL.FormatStyle.ComponentDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s scheme component in accordance with the provided option.

func user(URL.FormatStyle.ComponentDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s user component in accordance with the provided option.

func password(URL.FormatStyle.ComponentDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s password component in accordance with the provided option.

func host(URL.FormatStyle.HostDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s host component in accordance with the provided option.

struct HostDisplayOption

A type that indicates whether a formatted URL should include the host component.

func port(URL.FormatStyle.ComponentDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s port component in accordance with the provided option.

func query(URL.FormatStyle.ComponentDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s query component in accordance with the provided option.

func fragment(URL.FormatStyle.ComponentDisplayOption) -> URL.FormatStyle

Modifies a format style to display a URL’s fragment component in accordance with the provided option.

struct ComponentDisplayOption

A type that indicates whether a formatted URL should include a component.

