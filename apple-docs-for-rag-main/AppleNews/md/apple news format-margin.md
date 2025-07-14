

- Apple News Format
-  Margin 

Object

# Margin

The object for defining the space above and below a component.

Apple News Format 1.7+

``` source
object Margin
```

## Properties

`bottom`

`(`SupportedUnits` | number)`

The bottom margin in `points`, or with any of the units of measure for components. See Specifying Measurements for Components.

Possible types: SupportedUnits`, ``number`

`top`

`(`SupportedUnits` | number)`

The top margin in `points`, or with any of the units of measure for components. See Specifying Measurements for Components.

Possible types: SupportedUnits`, ``number`

## Mentioned in 

Positioning the Content in Your Article

## Discussion

Use the `margin` object to specify top and bottom margins to designate space above and below a component. For information on the units, see Specifying Measurements for Components.

You can use this object in ComponentLayout and AutoPlacementLayout.

### Example

```
{
  "components": [
    {
      "role": "header",
      "layout": "headerLayout",
      "components": [
        {
          "role": "title",
          "text": "Article Title"
        }
      ]
    }
  ],
  "componentLayouts": {
    "headerLayout": {
      "margin": {
        "top": 50,
        "bottom": 50
      }
    }
  }
}
```

## See Also

### Article Layout

Planning the Layout for Your Article

Define a layout that supports the look you want for your article.

Positioning the Content in Your Article

Align article components with columns in your layout.

Wrapping Text Around a Component

Define the layout of a text component to wrap around another component.

object Layout

The object for defining columns, gutters, and margins for your article’s designed width.

object ComponentLayout

The object for defining the positioning for a specific component within the article’s column system.

object Anchor

The object for anchoring one component to another component in your article’s layout.

object AutoPlacementLayout

The object for defining the margin above and below advertising components.

object AdvertisingLayout

The object for defining the margin above and below advertising components.

Deprecated

