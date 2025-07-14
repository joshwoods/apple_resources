

- Apple News Format
-  ConditionalSection 

Object

# ConditionalSection

The object for defining conditional properties for a section component, and when the conditional properties are in effect.

Apple News Format 1.9+

``` source
object ConditionalSection
```

## Properties

`conditions`

`(`Condition` | [`Condition`])`

 (Required) 

An instance or array of conditions that, when met, cause the conditional section component properties to take effect.

Possible types: Condition`, ``[`Condition`]`

`allowAutoplacedAds`

`boolean`

A Boolean value that allows the placement of ad banners between components. Nested components inherit the value of the outermost container that explicitly sets `allowAutoplacedAds`. The default value is `true`.

Default: `true`

`anchor`

Anchor

An object that defines vertical alignment with another component.

`animation`

`(`ComponentAnimation` | string("none"))`

An object that defines an animation to apply to the component.

To remove a previously set condition, use `none`.

Possible types: ComponentAnimation`, ``string("none")`

`behavior`

`(`Behavior` | string("none"))`

An object that defines behavior for a component, like Parallax or Springy.

To remove a previously set condition, use `none`.

Possible types: Behavior`, ``string("none")`

`contentDisplay`

`(`CollectionDisplay` | `HorizontalStackDisplay` | string("none"))`

An object that defines how to position child components within this `ConditionalSection` component. A HorizontalStackDisplay, for example, allows for displaying child components side by side.

To remove a previously set condition, use `none`.

Possible types: CollectionDisplay`, `HorizontalStackDisplay`, ``string("none")`

`hidden`

`boolean`

A Boolean value that determines whether the component is hidden.

Default: `false`

`layout`

`(`ComponentLayout` | string)`

An inline ComponentLayout object that contains layout information, or a string reference to a `ComponentLayout` object that you define at the top level of the document.

If you don’t define `layout`, Apple News bases the size and position on various factors, such as the device type, the length of the content, and the `role` of this component.

Possible types: ComponentLayout`, ``string`

`scene`

`(`Scene` | string("none"))`

A set of animations applied to any header component that’s a child of this section.

To remove a previously set condition, use `none`.

Possible types: Scene`, ``string("none")`

`style`

`(`ComponentStyle` | string | string("none"))`

An inline ComponentStyle object that defines the appearance of this component, or a string reference to a `ComponentStyle` object that you define at the top level of the document.

To remove a previously set condition, use `none`.

Possible types: ComponentStyle`, ``string``, ``string("none")`

## Discussion

Use the `ConditionalSection` object to define an array of conditional section properties and the conditions under which to apply them. When a condition is met, the value of a property in `ConditionalSection` overrides the value of the same property if defined in the parent `Section` component. See Section.

### Example

```
{
  "components": [
    {
      "role": "section",
      "components": [
        {
          "role": "photo",
          "URL": "bundle://header.jpg"
        },
        {
          "role": "title",
          "text": "Section Title Beneath Image"
        }
      ],
      "hidden": true,
      "conditional": [
        {
          "hidden": false,
          "conditions": [
            {
              "maxViewportWidth": 415
            }
          ]
        }
      ]
    },
    {
      "role": "section",
      "components": [
        {
          "role": "header",
          "style": {
            "fill": {
              "type": "image",
              "URL": "bundle://header.jpg"
            }
          },
          "layout": {
            "minimumHeight": "75cw"
          },
          "components": [
            {
              "role": "title",
              "text": "Section Title Overlay",
              "anchor": {
                "targetAnchorPosition": "center"
              }
            }
          ]
        }
      ],
      "hidden": true,
      "conditional": [
        {
          "hidden": false,
          "conditions": [
            {
              "minViewportWidth": 416
            }
          ]
        }
      ]
    }
  ]
}
```

## Relationships

### Inherits From

- ConditionalContainer

## See Also

### Conditional Design Elements

object Condition

The object for defining a condition that, when met, causes conditional properties to go into effect.

object ConditionalComponent

The object for defining conditional properties for a component, and when the conditional properties are in effect.

object ConditionalComponentLayout

The object for defining conditional properties for a component layout, and when the conditional properties are in effect.

object ConditionalAutoPlacement

The object for defining conditional properties for an automatically placed component, and when the conditional properties are in effect.

object ConditionalDocumentStyle

The object for defining conditional properties for a document style, and when the conditional properties are in effect.

object ConditionalText

The object for defining conditional properties for a text component, and when the conditional properties are in effect.

object ConditionalTextStyle

The object for defining conditional properties for a text style, and when the conditional properties are in effect.

object ConditionalComponentTextStyle

The object for defining conditional properties for a component text style, and when the conditional properties are in effect.

object ConditionalComponentStyle

The object for defining conditional properties for a component style, and when the conditional properties are in effect.

object ConditionalContainer

The object for defining conditional properties for a container component, and when the conditional properties are in effect.

object ConditionalDivider

The object for defining conditional properties for a divider component, and when the conditional properties are in effect.

object ConditionalButton

The object for defining a button component’s conditional properties, and when the conditional properties are in effect.

