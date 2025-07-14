

- Apple News Format
-  Anchor 

Object

# Anchor

The object for anchoring one component to another component in your article’s layout.

Apple News Format 1.7+

``` source
object Anchor
```

## Properties

`targetAnchorPosition`

`string`

 (Required) 

Sets the anchor point in the target component, relative to the `originAnchorPosition`. Valid values:

- `top`: Align the top of the target component with or near the `originAnchorPosition`.

- `center`: Align the middle of the target component with or near the `originAnchorPosition`.

- `bottom`: Align the bottom of the target component with or near the `originAnchorPosition`.

If a component is anchored to a range of text in a body component and is full-width (such as iPhone), the following rules determine the spacing before and after the anchored component:

- If the anchored component has explicitly defined margins, Apple News Format applies the defined margins to the component.

- If the anchored component doesn’t have explicitly defined margins, Apple News Format adds space equaling half of the document gutter before and after the component.

Note the following:

- If you anchor the component to a range of text near the beginning of the component and it appears above all text in the body component, Apple News Format doesn’t add any space above it.

- If you anchor the component to a range of text near the end of the component and it appears after all text in the body component, Apple News Format doesn’t add any space after it.

- If the component’s `targetAnchorPosition` is `top`, Apple News Format doesn’t add any space above it.

- If the component’s `targetAnchorPosition` is `bottom`, Apple News Format doesn’t add any space after it.

Example: To align the bottom of a component with the bottom of another component, set both `originAnchorPosition` and `targetAnchorPosition` to `bottom`.

Possible Values: `top, center, bottom`

`originAnchorPosition`

`string`

Sets which point in the origin component gets anchored to the target component. The originating anchor is positioned as closely as possible to the intended `targetAnchorPosition`. If you omit this property, Apple News uses the value of `targetAnchorPosition`.

Possible Values: `top, center, bottom`

`rangeLength`

`integer`

The length of the range of text the component is anchored to. If you specify `rangeLength`, you must include `rangeStart`.

Maximum value: (`textLength` - `rangeStart`) where `textLength` is the number of characters in the component, including spaces.

The length of a text range can’t exceed the length of the text.

`rangeStart`

`integer`

The start index of the range of text the component is anchored to. When a component is anchored to a component with a `role` of `body`, Apple News Format might flow text around the component.

If you specify `rangeStart`, you must include `rangeLength`.

`target`

`string`

The id or name attribute of an `HTML` element in another component. Set the component containing the target element to `html`.

`targetComponentIdentifier`

`string`

The identifier of the component to anchor to. `targetComponentIdentifier` can’t refer to the current component’s parent, child components, or components in another container. If you omit this property, Apple News Format applies the anchor to the parent component, if one exists.

If a parent component doesn’t exist and you don’t specify the `targetComponentIdentifier`, Apple News Format ignores the anchor.

## Mentioned in 

Positioning the Content in Your Article

Wrapping Text Around a Component

## Discussion

Use the `Anchor` object to anchor one component (called the *origin*) to another component (called the *target*). You can use an anchor to align components vertically. For example, you can anchor a `caption` component to a `photo` component and choose whether you want the caption aligned to the top, bottom, or center of the photograph. You can also use an anchor to position a child component within its parent container. For information about using anchors within containers, see Nesting Components in an Article.

Note

The vertical placement of the anchored components can vary on different devices depending on the size of the display area of the device.

You can use this object in Component.

### Example

```
{
  "components": [
    {
      "role": "container",
      "layout": {
        "minimumHeight": 100
      },
      "style": {
        "backgroundColor": "goldenrod"
      },
      "components": [
        {
          "role": "title",
          "text": "Article Title",
          "anchor": {
            "targetAnchorPosition": "bottom"
          }
        }
      ]
    }
  ]
}
```

## See Also

### Related Documentation

Creating a Floating Caption

Position a caption in the wide right margin of your article.

Creating an Inset Pull Quote

Wrap article body text around an inset pull quote.

Creating an Inset Photo

Wrap article body text around an inset photo.

Creating a Sidebar

Create a box with an HTML bulleted list in the margin.

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

object Margin

The object for defining the space above and below a component.

object AutoPlacementLayout

The object for defining the margin above and below advertising components.

object AdvertisingLayout

The object for defining the margin above and below advertising components.

Deprecated

