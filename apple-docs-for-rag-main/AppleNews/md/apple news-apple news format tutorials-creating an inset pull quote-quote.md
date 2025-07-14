

- Apple News
- Apple News Format Tutorials
-  Creating an Inset Pull Quote 

Article

# Creating an Inset Pull Quote

Wrap article body text around an inset pull quote.

## Overview

In Creating a Floating Caption, you positioned a component in the article margin. Now, you’ll position a component in the same columns as the body text and make text wrap around it.

**On this page, you’ll learn how to:**

- Enclose the `pullquote` components in a container so that you can position the components as one unit.

- Use a `ComponentLayout` object to control the horizontal placement of the container.

- Use an anchor to control vertical placement and allow body text to flow around the pull quote.

- Delete some `divider` components, and replace them with top and bottom borders.

### Define Minor Adjustments for Pull Quote Position

Before you can position the pull quote in the leftmost three columns of the article, you must define some new `ComponentLayout` objects. The `quoteLockupLayout` object determines that the pull quote is displayed in the left portion of the article. The other two `ComponentLayout` objects will make minor vertical adjustments to the components’ placement.

Tip

Two of the `ComponentLayout` objects in this example only have a `margin` property. Because the `columnStart` and `columnSpan` properties are not specified, these `ComponentLayout` objects will always extend to the left and right margins of the available space (either the parent container, or the whole article if there is no parent container). You can reuse margin-only `ComponentLayout` objects like these to adjust vertical positioning within containers, and then use the containers’ `ComponentLayout` objects to adjust other aspects of the layout.

1.  Copy the example code Inset Pull Quote Layout: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentLayout` object and the closing brace for the whole `componentLayouts` property.

Your code should look like the example code Inset Pull Quote Layout: Result.

#### Inset Pull Quote Layout: Copy This Code

```
,
    "quoteLockupLayout": {
      "columnStart": 0,
      "columnSpan": 6
    },
    "halfMarginAboveQuarterBelowContainedLayout": {
      "margin": {
        "top": 12,
        "bottom": 6
      }
    },
    "halfMarginBelowContainedLayout": {
      "margin": {
        "bottom": 12
      }
    }
```

#### Inset Pull Quote Layout: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentLayouts": {
    ...
    "quoteLockupLayout": {
      "columnStart": 0,
      "columnSpan": 6
    },
    "halfMarginAboveQuarterBelowContainedLayout": {
      "margin": {
        "top": 12,
        "bottom": 6
      }
    },
    "halfMarginBelowContainedLayout": {
      "margin": {
        "bottom": 12
      }
    }
  },
  ...
}
```

### Create Top and Bottom Borders

Your pull quote has dividers above and below it, and you’ll replace these with borders. Before you can add top and bottom borders to the pull quote, you must create a `ComponentStyle` object that creates a top and bottom border.

1.  Copy the example code quoteLockupStyle: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentStyle` object and the closing brace for the whole `componentStyles` property.

Your code should look like the example code quoteLockupStyle: Result.

#### quoteLockupStyle: Copy This Code

```
,
    "quoteLockupStyle": {
      "border": {
        "all": {
          "width": 1,
          "color": "#D5B327"
        },
        "top": true,
        "right": false,
        "bottom": true,
        "left": false
      }
    }
```

#### quoteLockupStyle: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentStyles": {
    ...
    "quoteLockupStyle": {
      "border": {
        "all": {
          "width": 1,
          "color": "#D5B327"
        },
        "top": true,
        "right": false,
        "bottom": true,
        "left": false
      }
    }
  },
  ...
}
```

### Recombine Body Components and Use Style and Layout with a Container

1.  In your `article.json` file, copy the value of `text` for the first `body` component whose text begins with `Quis autem vel eum`. Do not copy the quotation marks.

2.  Paste the text inside the value of `text` for the `body` component whose text begins with `Cras ultricies mi eu turpis`, at the beginning of the value, before the existing `.` Then wrap the pasted text with ``.

3.  In your `article.json` file, delete the first `body` component whose text begins with `Quis autem vel eum`. This is the component you copied from in step 1.

4.  In your `article.json` file, delete the two `pullquote` components and the dividers that precede and follow them. The code you’re deleting begins with an opening brace (`{`) before `"role": "divider",` and ends with a closing brace and a comma (`},`).

5.  Copy the example code Container: Copy This Code.

6.  Paste the code after the closing brace (`}`) of the `body` component whose text begins with `Quis autem vel eum`.

Your code should look like the example code Container: Result.

After you make this change in your code, you can preview your working `article.json` file in News Preview to see that the pull quote is vertically aligned. Note that the text does not yet wrap around the pull quote.

#### Container: Copy This Code

```
        {
          "role": "container",
          "layout": "quoteLockupLayout",
          "style": "quoteLockupStyle",
          "components": [
            {
              "role": "pullquote",
              "format": "html",
              "layout": "halfMarginAboveQuarterBelowContainedLayout",
              "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
            },
            {
              "role": "pullquote",
              "layout": "halfMarginBelowContainedLayout",
              "textStyle": "attribution",
              "text": "— ATTRIBUTION"
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
          "layout": "quoteLockupLayout",
          "style": "quoteLockupStyle",
          "components": [
            {
              "role": "pullquote",
              "format": "html",
              "layout": "halfMarginAboveQuarterBelowContainedLayout",
              "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
            },
            {
              "role": "pullquote",
              "layout": "halfMarginBelowContainedLayout",
              "textStyle": "attribution",
              "text": "— ATTRIBUTION"
            }
          ]
        },
        ...
      ]
    }
  ],
  ...
}
```

### Wrap Text Around the Pull Quote

Now that the `pullquote` components are combined in a container, you can use HTML to anchor the container, as one unit, to a portion of the body text.

To create an anchor to a location in a `body` component, you’ll define the target inline in the HTML.

1.  Copy the example code Anchor: Copy This Code.

2.  Paste the code inside the `container` component that encloses the `pullquote` components, after this line: `"style": "quoteLockupStyle",`

3.  Copy the code ``

4.  Paste the code inside the `body` component whose text begins with `Quis autem vel eum`, replacing a `` tag, as in the example code Anchor: Result. You may have to scroll to the right in the example code to see this.

Your code should look like the example code Anchor: Result.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see the text wrapped around the pull quote.

#### Anchor: Copy This Code

```
          "anchor": {
            "targetAnchorPosition": "center",
            "target": "p1"
          },
```

#### Anchor: Result

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
          "layout": "quoteLockupLayout",
          "style": "quoteLockupStyle",
          "anchor": {
            "targetAnchorPosition": "center",
            "target": "p1"
          },
          "components": [
            {
              "role": "pullquote",
              "format": "html",
              "layout": "halfMarginAboveQuarterBelowContainedLayout",
              "text": "“QUIA CONSEQUUNTUR MAGNI DOLORES EOS QUI RATIONE VOLUPTATEM SEQUI NESCIUNT.”"
            },
            {
              "role": "pullquote",
              "layout": "halfMarginBelowContainedLayout",
              "textStyle": "attribution",
              "text": "— ATTRIBUTION"
            }
          ]
        },
        {
          "role": "body",
          "format": "html",
          "layout": "noMarginLayout",
          "text": "Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur? At vero eos et accusamus et iusto odio ducimus qui blanditiis.Cras ultricies mi eu turpis hendrerit fringilla. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; In ac dui quis mi consectetuer.Temporibus autem et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae sint et molestiae non recusandae. Itaque rerum hic tenetur.Inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo esciunt enim ipsam voluptatem quia.Ut aut reiciendis voluptatibus maiores alias consequatur aut perferendis link text repellat. Sed ut perspiciatis unde omnis iste natus sit voluptatem accusantium doloremque, totam rem aperiam, eaque ipsa quae ab illo inventore.Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni."
        },
        ...
      ]
    }
  ],
  ...
}
```

### Previous

Creating a Floating Caption

### Next

Creating an Inset Photo

## See Also

### Related Documentation

Positioning the Content in Your Article

Align article components with columns in your layout.

Wrapping Text Around a Component

Define the layout of a text component to wrap around another component.

Nesting Components in an Article

Use container components to create the component hierarchies you need for special article designs.

object Anchor

The object for anchoring one component to another component in your article’s layout.

object ComponentStyle

The object for setting style properties for components, including background color and fill, borders, and table styles.

object Border

The object for setting borders for component sides or tables.

object StrokeStyle

The object for defining the color, width, and style of a border or divider.

### Advanced Design Tutorial 2: Layout and Positioning

Creating a Complex, Layered Header

Layer a title and heading in front of an image, with their colors optimized for legibility.

Creating a Floating Caption

Position a caption in the wide right margin of your article.

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

