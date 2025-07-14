

- Group Activities
- SpatialTemplatePreference
-  conversational 

Type Property

# conversational

An arrangement where the participants can see one another and the app’s content.

visionOS 1.0+

``` source
static let conversational: SpatialTemplatePreference
```

## Discussion

This arrangement works best when you want participants to converse with each other and also look at your app’s content.

For example:

```
      App

A             C

       B
```

## See Also

### Getting the spatial position preferences

static let none: SpatialTemplatePreference

An arrangement where the system places spatial Personas based on your app’s content.

static let sideBySide: SpatialTemplatePreference

An arrangement where the participants sit in a line with the content in front of them.

static func custom(any SpatialTemplate) -> SpatialTemplatePreference

Creates a template preference with the given custom spatial template.

