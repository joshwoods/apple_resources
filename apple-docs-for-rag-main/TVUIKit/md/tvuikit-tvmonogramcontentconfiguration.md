

- TVUIKit
-  TVMonogramContentConfiguration 

Structure

# TVMonogramContentConfiguration

A content configuration for a monogram view.

tvOS 15.0+

``` source
struct TVMonogramContentConfiguration
```

## Topics

### Creating Default Configurations

static func cell() -> TVMonogramContentConfiguration

Creates the default configuration for a circular monogram cell.

### Customizing Content

var image: UIImage?

The image to display.

var text: String?

The primary text.

var secondaryText: String?

The secondary text.

var personNameComponents: PersonNameComponents?

The name the system uses when creating a monogram image.

### Customizing Appearance

var textProperties: TVMonogramContentConfiguration.TextProperties

Properties for configuring the primary text.

var secondaryTextProperties: TVMonogramContentConfiguration.TextProperties

Properties for configuring the secondary text.

struct TextProperties

Properties that affect the monogram content configuration’s text.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- UIContentConfiguration

## See Also

### Creating a Monogram Content View

convenience init(configuration: TVMonogramContentConfiguration)

Creates a monogram content view with the configuration you specify.

