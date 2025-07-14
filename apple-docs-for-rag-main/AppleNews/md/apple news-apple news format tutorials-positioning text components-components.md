

- Apple News
- Apple News Format Tutorials
-  Positioning Text Components 

Article

# Positioning Text Components

Adjust the positions of the text components in your article—for example, place the article body off-center.

## Overview

In Creating Your First Article, you added some text components and component text styles to your article.

**On this page, you’ll learn how to control:**

- Where text components are horizontally aligned

- How wide the text components are

- The vertical spacing between the text components

### Define Basic ComponentLayout Objects

`ComponentLayout` objects determine the placement of components in your article.

1.  Copy the example code Basic ComponentLayout Objects: Copy This Code.

2.  In your `article.json` file, select this line: `"componentLayouts": {},`

3.  Paste the copied code into `article.json`, replacing the line that you selected in the previous step.

Note

The names of these `ComponentLayout` objects were created for this tutorial; when you create your own articles, you can create your own `ComponentLayout` object names. For the purposes of this tutorial, a “full” margin was considered to be a 24-point space above a or below a component, a “half” margin to be a 12-point space, and a “quarter” margin to be a 6-point space.

#### Basic ComponentLayout Objects: Copy This Code

```
  "componentLayouts": {
    "noMarginLayout": {
      "columnStart": 0,
      "columnSpan": 14
    },
    "heading1Layout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "top": 24,
        "bottom": 3
      }
    },
    "halfMarginBelowLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "bottom": 12
      }
    },
    "fullMarginBelowLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "bottom": 24
      }
    },
    "fullMarginAboveHalfBelowLayout": {
      "columnStart": 0,
      "columnSpan": 14,
      "margin": {
        "top": 24,
        "bottom": 12
      }
    }
  },
```

### Use ComponentLayout Objects in Text Components

Now that you have defined some `ComponentLayout` objects, you can use them in one or more components.

Add references to `ComponentLayout` objects inside components as shown in the example code Positioning Text Components: Result. In each object, use `"layout"` as the property name and the name of the `ComponentLayout` object as the property value.

After you make this change in your code, you can preview your working `article.json` file in News Preview to see changes in the positioning of your components. For example, your article now has a wide right margin when viewed on an iPad.

#### Positioning Text Components: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "heading1",
      "layout": "heading1Layout",
      "text": "HEADING"
    },
    {
      "role": "title",
      "layout": "halfMarginBelowLayout",
      "text": "ARTICLE TITLE"
    },
    {
      "role": "intro",
      "layout": "halfMarginBelowLayout",
      "text": "Etiam rhoncus. Maecenas tempus, tellus eget condimentum rhoncus, sem quam semper libero, sit amet adipiscing sem neque ipsum?"
    },
    {
      "role": "byline",
      "layout": "fullMarginBelowLayout",
      "text": "By Urna Semper"
    },
    {
      "role": "body",
      "format": "html",
      "layout": "noMarginLayout",
      "textStyle": "bodyFirstDropCap",
      "text": "Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas assumenda est, dolor repellendus. Link text quibusdam et aut.Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, adipisci velit."
    },
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "LOREM IPSUM DOLOR"
    },
    {
      "role": "body",
      "format": "html",
      "layout": "noMarginLayout",
      "text": "Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur? At vero eos et accusamus et iusto odio ducimus qui blanditiis.Cras ultricies mi eu turpis hendrerit fringilla. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; In ac dui quis mi consectetuer.Temporibus autem et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae sint et molestiae non recusandae. Itaque rerum hic tenetur.Inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo esciunt enim ipsam voluptatem quia.Ut aut reiciendis voluptatibus maiores alias consequatur aut perferendis link text repellat. Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque, totam rem aperiam, eaque ipsa quae ab illo inventore.Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni."
    },
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "HEADING"
    },
    {
      "role": "body",
      "format": "html",
      "layout": "noMarginLayout",
      "text": "Sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas."
    },
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "HEADING"
    },
    {
      "role": "body",
      "format": "html",
      "layout": "noMarginLayout",
      "text": "Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas est, omnis dolor repellendus."
    },
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "HEADING"
    },
    {
      "role": "body",
      "format": "html",
      "layout": "noMarginLayout",
      "text": "Consequatur aut doloribus asperiores repellat. Sed ut perspiciatis unde omnis iste natus error sit volup tatem accusantium doloremque laudantium, totam rem, eaque ipsa quae ab illo inventore veritatis et quasi archit ecto beatae vitae.Nemo enim ipsam volup tatem quia voluptas sit aspernatur aut odit aut fugit, sed quia conse quuntur magni. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam.Consequatur aut perferendis doloribus asperiores repellat. Sed ut perspiciatis unde omnis iste natus error sit volup tatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi archit ecto beatae vitae dicta. Nemo enim ipsam volup tatem quia voluptas sit link text aut odit aut fugit, sed quia conse quuntur perspiciatis doloribus magni dolores.Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam suscipit laboriosam."
    },
    {
      "role": "heading2",
      "layout": "fullMarginAboveHalfBelowLayout",
      "text": "HEADING"
    },
    {
      "role": "body",
      "format": "html",
      "layout": "noMarginLayout",
      "text": "Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur? At vero eos et accusamus et iusto odio. Dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati."
    },
  ],
  ...
}
```

### Previous

Creating Your First Article

### Next

Adding a Divider

## See Also

### Related Documentation

Positioning the Content in Your Article

Align article components with columns in your layout.

object ComponentLayout

The object for defining the positioning for a specific component within the article’s column system.

Planning the Layout for Your Article

Define a layout that supports the look you want for your article.

### Introductory Design Tutorial

Setting Up the Introductory Tutorial

Download the tutorial files, and learn about what you’ll create in the introductory tutorial.

Creating Your First Article

Create an article with text components and component text styles.

Adding a Divider

Create a horizontal, styled divider that extends to the right edge of the display.

Adding an Image and Captions

Create a photo that extends to both edges of the display, with captions that appear in the article layout and in full-screen view.

Adding a Pull Quote

Break an existing body component into two components, and then insert a pull quote between them.

Adding a Gallery of Images

Display three images as a sequential gallery.

Adding a Mosaic of Images

Display five images as mosaic tiles.

Adding a Tweet

Include a tweet in an article.

Adding a Podcast

Add a link to a podcast that displays the podcast artwork and the podcast show or episode information.

Viewing the Finished Article for the Introductory Design Tutorial

See the full JSON code from this tutorial.

