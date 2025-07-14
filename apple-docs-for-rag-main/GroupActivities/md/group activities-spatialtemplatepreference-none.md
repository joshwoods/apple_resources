

- Group Activities
- SpatialTemplatePreference
-  none 

Type Property

# none

An arrangement where the system places spatial Personas based on your app’s content.

visionOS 1.0+

``` source
static let none: SpatialTemplatePreference
```

## Discussion

With this option, the system examines your app’s content to determine the best arrangement. For content in a vertical plane such as a window, the system arranges participants side by side and facing the content. For volumes, the system surrounds the volume with the participants. This option is the default.

## See Also

### Getting the spatial position preferences

static let sideBySide: SpatialTemplatePreference

An arrangement where the participants sit in a line with the content in front of them.

static let conversational: SpatialTemplatePreference

An arrangement where the participants can see one another and the app’s content.

static func custom(any SpatialTemplate) -> SpatialTemplatePreference

Creates a template preference with the given custom spatial template.

