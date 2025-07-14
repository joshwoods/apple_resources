

- Group Activities
- SpatialTemplatePreference
-  sideBySide 

Type Property

# sideBySide

An arrangement where the participants sit in a line with the content in front of them.

visionOS 1.0+

``` source
static let sideBySide: SpatialTemplatePreference
```

## Discussion

The participants are side by side and face your app’s shared content. This arrangement works best for windows and other vertically oriented content. For example, you might use it for a group of participants watching a movie. However, you can apply it to any for other content configurations.

For example:

```
        App

A     B     C     D
```

## See Also

### Getting the spatial position preferences

static let none: SpatialTemplatePreference

An arrangement where the system places spatial Personas based on your app’s content.

static let conversational: SpatialTemplatePreference

An arrangement where the participants can see one another and the app’s content.

static func custom(any SpatialTemplate) -> SpatialTemplatePreference

Creates a template preference with the given custom spatial template.

