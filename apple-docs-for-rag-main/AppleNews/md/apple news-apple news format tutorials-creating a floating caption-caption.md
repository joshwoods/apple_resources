

- Apple News
- Apple News Format Tutorials
-  Creating a Floating Caption 

Article

# Creating a Floating Caption

Position a caption in the wide right margin of your article.

## Overview

Apple News Format makes it easy to create side-by-side content, such as a caption that floats next to the article body. On sufficiently wide displays, News automatically lays out such a caption in the article margin; on narrower displays, News automatically stacks the caption with other article content.

**On this page, you’ll learn how to create a caption that appears in the right margin of the article on wide displays.**

### Create a ComponentLayout Object for the Floating Caption

Before you can position the caption in the right margin, you must define a component layout object that specifies that the caption will begin in column 7 of the article layout and span three columns.

1.  Copy the example code sideCaptionLayout: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentLayout` object and the closing brace for the whole `componentLayouts` property.

Your code should look like the example code sideCaptionLayout: Result.

#### sideCaptionLayout: Copy This Code

```
,
    "sideCaptionLayout": {
      "columnStart": 14,
      "columnSpan": 6,
      "margin": {
        "bottom": 24
      }
    }
```

#### sideCaptionLayout: Result

```
{
  ...
  "componentLayouts": {
    ...
    "sideCaptionLayout": {
      "columnStart": 14,
      "columnSpan": 6,
      "margin": {
        "bottom": 24
      }
    }
  },
  ...
}
```

### Anchor the Caption to the Article Body

On wide displays, when you anchor a caption to the article body, the caption’s top edge will be aligned with the body’s top edge; on narrower displays, the caption will be stacked above the body.

1.  Delete the `caption` component and its parent container from your header.  The code you’re deleting begins with the comma and opening brace (,`{`) before `"role": "container",` and ends with a mix of three alternating braces and brackets, and a comma (`}]}`).

2.  Copy the example code Caption: Copy This Code.

3.  Paste the code inside your article’s second section, before the opening brace (`{`) of the `body` component whose text begins with `Nam libero tempore`.

4.  Inside the `body` component whose text begins with `Nam libero tempore`, add an `identifier` property with a value of `"body1"`, as shown in the example code Caption: Result.

After you make these changes in your `article.json` file, you can preview your working `article.json` file in News Preview to see the floating caption.

#### Caption: Copy This Code

```
        {
          "role": "container",
          "layout": "sideCaptionLayout",
          "anchor": {
            "targetComponentIdentifier": "body1",
            "targetAnchorPosition": "top",
            "originAnchorPosition": "top"
          },
          "components": [
            {
              "role": "caption",
              "format": "html",
              "layout": "fullBleedLayout",
              "text": "ABOVE: Sed ut pers piciatis unde omnis iste error sit volup tatem accusa ntium dolor emque, totam rem. (Attribution)"
            }
          ]
        },
```

#### Caption: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "section",
      ...
      "components": [
        ...
        {
          "role": "container",
          "layout": "sideCaptionLayout",
          "anchor": {
            "targetComponentIdentifier": "body1",
            "targetAnchorPosition": "top",
            "originAnchorPosition": "top"
          },
          "components": [
            {
              "role": "caption",
              "format": "html",
              "layout": "fullBleedLayout",
              "text": "ABOVE: Sed ut pers piciatis unde omnis iste error sit volup tatem accusa ntium dolor emque, totam rem. (Attribution)"
            }
          ]
        },
        {
          "identifier": "body1",
          "role": "body",
          "format": "html",
          "layout": "noMarginLayout",
          "textStyle": "bodyFirstDropCap",
          "text": "Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas assumenda est, dolor repellendus. Link text quibusdam et aut.Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, adipisci velit."
        },
        ...
      ]
    }
  ],
  ...
}
```

### Previous

Creating a Complex, Layered Header

### Next

Creating an Inset Pull Quote

## See Also

### Related Documentation

Planning the Layout for Your Article

Define a layout that supports the look you want for your article.

Positioning the Content in Your Article

Align article components with columns in your layout.

Wrapping Text Around a Component

Define the layout of a text component to wrap around another component.

Nesting Components in an Article

Use container components to create the component hierarchies you need for special article designs.

object Caption

The component for adding caption text.

object Layout

The object for defining columns, gutters, and margins for your article’s designed width.

object ComponentLayout

The object for defining the positioning for a specific component within the article’s column system.

object Anchor

The object for anchoring one component to another component in your article’s layout.

### Advanced Design Tutorial 2: Layout and Positioning

Creating a Complex, Layered Header

Layer a title and heading in front of an image, with their colors optimized for legibility.

Creating an Inset Pull Quote

Wrap article body text around an inset pull quote.

Creating an Inset Photo

Wrap article body text around an inset photo.

Adding Color to Text Ranges

Create text in color by using HTML to refer to TextStyle objects.

Adding Animations

Use animations to affect how parts of your article come into view the first time they appear.

Adding a Scene

Control how the article’s opening section comes into view.

Viewing the Finished Article for Advanced Design Tutorial 2

See the full JSON code from this tutorial.

