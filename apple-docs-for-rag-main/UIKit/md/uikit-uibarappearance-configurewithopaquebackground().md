

- UIKit
- UIBarAppearance
-  configureWithOpaqueBackground() 

Instance Method

# configureWithOpaqueBackground()

Configures the bar appearance object with a set of opaque colors that are appropriate for the current theme.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func configureWithOpaqueBackground()
```

## Discussion

Calling this method replaces any previous values you specified for the bar appearance properties.

## See Also

### Resetting the appearance properties

func configureWithDefaultBackground()

Configures the bar appearance object with default background and shadow values.

func configureWithTransparentBackground()

Configures the bar appearance object with a transparent background and no shadow.

