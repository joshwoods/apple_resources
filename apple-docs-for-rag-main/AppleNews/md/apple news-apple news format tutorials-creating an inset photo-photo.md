

- Apple News
- Apple News Format Tutorials
-  Creating an Inset Photo 

Article

# Creating an Inset Photo

Wrap article body text around an inset photo.

## Overview

In Creating an Inset Pull Quote, you placed a pull quote within the article body.

**On this page, you’ll learn how to:**

- Place a photo within the article body.

- Use a `ComponentLayout` object to control horizontal placement in the column system.

- Add an anchor to control vertical placement and make text wrap around the photo.

### Define ComponentLayout Objects for an Inset Photo

Before you can position the photo inside the article body, you must define some new `ComponentLayout` objects for this example. The `smallImageLayout` object determines that the pull quote container gets laid out in the rightmost three columns of the article text. The other two `ComponentLayout` objects make minor vertical adjustments.

1.  Copy the example code Inset Photo Layout: Copy This Code.

2.  Paste the code between the closing brace (}) of the last `ComponentLayout` object and the closing brace for the whole `componentLayouts` property.

Your code should look like the example code Inset Photo Layout: Result.

#### Inset Photo Layout: Copy This Code

```
,
    "smallImageLayout": {
      "columnStart": 8,
      "columnSpan": 6
    },
    "halfMarginAboveContainedLayout": {
      "margin": {
        "top": 12
      }
    },
    "halfMarginBothContainedLayout": {
      "margin": {
        "top": 12,
        "bottom": 12
      }
    }
```

#### Inset Photo Layout: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentLayouts": {
    ...
    "smallImageLayout": {
      "columnStart": 8,
      "columnSpan": 6
    },
    "halfMarginAboveContainedLayout": {
      "margin": {
        "top": 12
      }
    },
    "halfMarginBothContainedLayout": {
      "margin": {
        "top": 12,
        "bottom": 12
      }
    }
  },
  ...
}
```

### Define a Bottom Border

Before you can add a bottom border to the inset photo, you must define a `ComponentStyle` object that creates a bottom border only.

1.  Copy the example code captionLockupStyle: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentStyle` object and the closing brace for the whole `componentStyles` property.

Your code should look like the example code captionLockupStyle: Result.

#### captionLockupStyle: Copy This Code

```
,
    "captionLockupStyle": {
      "border": {
        "all": {
          "width": 1,
          "color": "#D5B327"
        },
        "top": false,
        "right": false,
        "bottom": true,
        "left": false
      }
    }
```

#### captionLockupStyle: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentStyles": {
    ...
    "captionLockupStyle": {
      "border": {
        "all": {
          "width": 1,
          "color": "#D5B327"
        },
        "top": false,
        "right": false,
        "bottom": true,
        "left": false
      }
    }
  },
  ...
}
```

### Use Style and Layout, and Wrap Text Around a Container

In Download the Article Bundle Examples, you downloaded a bundle called `News_Design_Tutorial_Advanced_Article_2` that contains a sidebar image. Now, you’ll move that image into your working folder and create a photo component to display the image.

1.  Move the `sidebar.jpg` file from `Desktop/News_Design_Tutorial_Advanced/News_Design_Tutorial_Advanced_Article_2` folder to your working article directory. This directory is most likely `Desktop/News_Design_Tutorial_Advanced/News_Design_Tutorial_6_Embeds` or `Desktop/News_Design_Tutorial_Advanced/News_Design_Tutorial_Advanced_Article_1`.

2.  Copy the example code Container: Copy This Code.

3.  Paste the code before the opening brace (`{`) of the body component whose text begins with `Consequatur aut doloribus`.

4.  Copy the code ``

5.  Paste the code in the `body` component whose text begins with `Consequatur aut doloribus`, as in the example code Container: Result. You may have to scroll to the right in the example code to see this.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see the inset photo.

#### Container: Copy This Code

```
        {
          "role": "container",
          "layout": "smallImageLayout",
          "style": "captionLockupStyle",
          "anchor": {
            "targetAnchorPosition": "top",
            "originAnchorPosition": "top",
            "target": "a1"
          },
          "components": [
            {
              "role": "photo",
              "layout": "noMarginLayout",
              "URL": "bundle://sidebar.jpg",
              "caption": "A caption for the sidebar photo."
            },
            {
              "role": "caption",
              "format": "html",
              "layout": "halfMarginBothContainedLayout",
              "text": "ABOVE: A caption for the sidebar photo. (Attribution)"
            }
          ]
        },
```

#### Container: Result

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
          "layout": "smallImageLayout",
          "style": "captionLockupStyle",
          "anchor": {
            "targetAnchorPosition": "center",
            "target": "a1"
          },
          "components": [
            {
              "role": "photo",
              "layout": "halfMarginAboveContainedLayout",
              "URL": "bundle://sidebar.jpg",
              "caption": "A caption for the sidebar photo."
            },
            {
              "role": "caption",
              "format": "html",
              "layout": "halfMarginBothContainedLayout",
              "text": "ABOVE: A caption for the sidebar photo. (Attribution)"
            }
          ]
        },
        {
          "role": "body",
          "format": "html",
          "layout": "noMarginLayout",
          "text": "Consequatur aut doloribus asperiores repellat. Sed ut perspiciatis unde omnis iste natus error sit volup tatem accusantium doloremque laudantium, totam rem, eaque ipsa quae ab illo inventore veritatis et quasi archit ecto beatae vitae.Nemo enim ipsam volup tatem quia voluptas sit aspernatur aut odit aut fugit, sed quia conse quuntur magni. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam.Consequatur aut perferendis doloribus asperiores repellat. Sed ut perspiciatis unde omnis iste natus error sit volup tatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi archit ecto beatae vitae dicta. Nemo enim ipsam volup tatem quia voluptas sit link text aut odit aut fugit, sed quia conse quuntur perspiciatis doloribus magni dolores.Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam suscipit laboriosam."
        },
        ...
      ]
    }
  ],
  ...
}
```

### Previous

Creating an Inset Pull Quote

### Next

Adding Color to Text Ranges

## See Also

### Related Documentation

Positioning the Content in Your Article

Align article components with columns in your layout.

Wrapping Text Around a Component

Define the layout of a text component to wrap around another component.

Nesting Components in an Article

Use container components to create the component hierarchies you need for special article designs.

object Photo

The component for including a photograph.

object Container

Properties shared by all container types.

object Anchor

The object for anchoring one component to another component in your article’s layout.

object Border

The object for setting borders for component sides or tables.

### Advanced Design Tutorial 2: Layout and Positioning

Creating a Complex, Layered Header

Layer a title and heading in front of an image, with their colors optimized for legibility.

Creating a Floating Caption

Position a caption in the wide right margin of your article.

Creating an Inset Pull Quote

Wrap article body text around an inset pull quote.

Adding Color to Text Ranges

Create text in color by using HTML to refer to TextStyle objects.

Adding Animations

Use animations to affect how parts of your article come into view the first time they appear.

Adding a Scene

Control how the article’s opening section comes into view.

Viewing the Finished Article for Advanced Design Tutorial 2

See the full JSON code from this tutorial.

