

- Apple News Format
-  ConditionalDivider 

Object

# ConditionalDivider

The object for defining conditional properties for a divider component, and when the conditional properties are in effect.

Apple News Format 1.10+

``` source
object ConditionalDivider
```

## Properties

`conditions`

`(`Condition` | [`Condition`])`

 (Required) 

An instance or array of conditions that, when met, cause the conditional divider component properties to take effect.

Possible types: Condition`, ``[`Condition`]`

`anchor`

Anchor

An object that defines vertical alignment with another component.

`animation`

`(`ComponentAnimation` | string("none"))`

An object that defines an animation to apply to the component.

To remove a previously set condition, use none.

Possible types: ComponentAnimation`, ``string("none")`

`behavior`

`(`Behavior` | string("none"))`

An object that defines behavior for a component, like Parallax or Springy.

To remove a previously set condition, use `none`.

Possible types: Behavior`, ``string("none")`

`hidden`

`boolean`

A Boolean value that determines whether the component is hidden.

Default: `false`

`layout`

`(`ComponentLayout` | string)`

An inline ComponentLayout object that contains layout information, or a string reference to a `ComponentLayout` object that you define at the top level of the document.

If you don’t define `layout`, Apple News bases the size and position on various factors, such as the device type, the length of the content, and the `role` of this component.

Possible types: ComponentLayout`, ``string`

`stroke`

`(`StrokeStyle` | string("none"))`

An object that defines the color, width, and style of a divider.

To remove a previously set condition, use `none`.

Possible types: StrokeStyle`, ``string("none")`

`style`

`(`ComponentStyle` | string | string("none"))`

An inline ComponentStyle object that defines the appearance of this component, or a string reference to a `ComponentStyle` object that you define at the top level of the document.

To remove a previously set condition, use `none`.

Possible types: ComponentStyle`, ``string``, ``string("none")`

## Discussion

Use the `ConditionalDivider` object to define an array of conditional divider properties and the conditions under which to apply them. When a condition is met, the value of a property in `ConditionalDivider` overrides the value of the same property if you define it in the parent `Divider` component. See Divider.

### Example

```
{
  "components": [
    {
      "role": "heading1",
      "text": "Heading"
    },
    {
      "role": "divider",
      "stroke": {
        "width": 3,
        "color": "#D5B327"
      },
      "conditional": {
        "stroke": {
          "color": "#d5263e"
        },
        "conditions": {
          "platform": "macos"
        }
      }
    }
  ]
}
```

## Relationships

### Inherits From

- ConditionalComponent

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

object ConditionalSection

The object for defining conditional properties for a section component, and when the conditional properties are in effect.

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

object ConditionalButton

The object for defining a button component’s conditional properties, and when the conditional properties are in effect.

