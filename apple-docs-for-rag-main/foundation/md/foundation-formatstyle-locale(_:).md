

- Foundation
- FormatStyle
-  locale(\_:) 

Instance Method

# locale(\_:)

Modifies the format style to use the specified locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func locale(_ locale: Locale) -> Self
```

**Required** Default implementation provided.

## Parameters 

`locale`  

The locale to apply to the format style.

## Return Value

A format style modified to use the provided locale.

## Discussion

Use this format style to change the locale used by an existing format style.

## Default Implementations

### FormatStyle Implementations

func locale(Locale) -> Self

