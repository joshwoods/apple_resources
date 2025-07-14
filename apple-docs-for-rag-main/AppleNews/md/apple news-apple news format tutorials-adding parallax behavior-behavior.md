

- Apple News
- Apple News Format Tutorials
-  Adding Parallax Behavior 

Article

# Adding Parallax Behavior

Create an illusion of multiple flat layers by causing the article body to overlap the header as the user scrolls.

## Overview

**On this page, you’ll learn how to add parallax behavior to your article.**

You’ll first divide the article’s components into two sections. This requires moving a large amount of code. Then, you’ll simply add a `behavior` property on the upper section and complete the effect by giving the lower section an opaque background color.

### Divide the Article Content into Sections

Add sections to the article’s top-level `components` array and move all existing components into the new sections. This requires moving a large amount of code.

1.  Copy the example code Section Components: Copy This Code.

2.  Paste the code inside the article’s top-level `components` array, after the opening bracket (`[`).

3.  In your `article.json` file, cut your `header` component—including all its nested component arrays—to your clipboard. The code you are cutting begins with the opening brace (`{`) before `"role": "header"` and ends with a mix of five alternating braces and brackets (`}]}]}`).

4.  In your `article.json` file, select the ellipses (`...`) in the first section.

5.  Paste the copied code into `article.json`, replacing the line that you selected in the previous step.

6.  In your `article.json` file, cut all components after the second section to your clipboard. The code you are cutting begins with the opening brace (`{`) before `"role": "heading1",` and ends with the closing brace (`}`) that ends your `tweet` component.

7.  In your `article.json` file, select the ellipses (`...`) in the second section.

8.  Paste the copied code into `article.json`, replacing the line that you selected in the previous step.

9.  Delete the extra comma between the closing brace (`}`) that ends the second `section` component and the closing bracket (`]`) that ends the article’s top-level `components` array.

Your code should look like the example code Section Components: Result (Collapsed) and Section Components: Result (Expanded).

After you make these changes in your code, you can successfully preview your working `article.json` file in News Preview, but it won’t look any different until you add parallax behavior in Add Parallax Behavior in the First Section.

#### Section Components: Copy This Code

```
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "components": [
        ...
      ]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "components": [
        ...
      ]
    }
```

#### Section Components: Result (Collapsed)

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "components": [
        ...
      ]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "components": [
        ...
      ]
    }
  ],
  ...
}
```

#### Section Components: Result (Expanded)

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "components": [
        {
          "role": "header",
          "layout": "headerImageLayout",
          "style": {
            "fill": {
              "type": "image",
              "URL": "bundle://header.jpg",
              "fillMode": "cover",
              "verticalAlignment": "top",
              "horizontalAlignment": "center"
            }
          },
          "components": [
            {
              "role": "container",
              "layout": "fullBleedLayout",
              "style": "captionBarBackgroundStyle",
              "anchor": {
                "targetAnchorPosition": "bottom"
              },
              "components": [
                {
                  "role": "caption",
                  "textStyle": "captionLight",
                  "layout": "halfMarginBothLayout",
                  "text": "ABOVE: Sed ut pers piciatis unde omnis iste error sit volup tatem accusantium dolor emque, totam rem. (Attribution)"
                }
              ]
            }
          ]
        }
      ]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "components": [
        {
          "role": "heading1",
          "layout": "heading1Layout",
          "text": "HEADING"
        },
        ...
        {
          "role": "tweet",
          "layout": "noMarginLayout",
          "URL": "https://twitter.com/Urna_Semper/status/1480968065630285834"
        }
      ]
    }
  ],
...
}
```

### Add Parallax Behavior in the First Section

Your article currently has two sections. You’ll use the first section’s `behavior` property to assign a parallax factor lower than 1, causing the first section to scroll more slowly than the default scroll speed.

1.  Copy the example code Behavior: Copy This Code.

2.  Paste the code inside the first `section` component, after the line `"layout": "fullBleedLayout",`

Your code should look like the example code Behavior: Result.

After you make this change in your code, you can preview your working `article.json` file in News Preview to see the changes in scroll speed. You might notice text becoming illegible as it covers the image. You’ll fix this in Use the Opaque Background with the Lower Section by adding a background color to the lower section.

#### Behavior: Copy This Code

```
      "behavior": {
        "type": "parallax",
        "factor": 0.8
      },
```

#### Behavior: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "behavior": {
        "type": "parallax",
        "factor": 0.8
      },
      "components": [
        {
          "role": "header",
          "layout": "headerImageLayout",
          "style": {
            "fill": {
              "type": "image",
              "URL": "bundle://header.jpg",
              "fillMode": "cover",
              "verticalAlignment": "top",
              "horizontalAlignment": "center"
            }
          },
          "components": [
            ...
          ]
        }
      ]
    },
    ...
  ],
  ...
}
```

### Define a ComponentStyle Object for Background Color

To finish the parallax behavior, you need to add a background color to the lower section. Before you can do that, you must define a `ComponentStyle` object.

1.  Copy the example code bodyBackgroundStyle: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentStyle` object and the closing brace for the whole `componentStyles` property.

Your code should look like the example code bodyBackgroundStyle: Result.

#### bodyBackgroundStyle: Copy This Code

```
,
    "bodyBackgroundStyle": {
      "backgroundColor": "#FFF"
    }
```

#### bodyBackgroundStyle: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentStyles": {
    ...
    "bodyBackgroundStyle": {
      "backgroundColor": "#FFF"
    }
  },
  ...
}
```

### Use the Opaque Background with the Lower Section

As a final step, you need to add a reference to the `ComponentStyle` object you just defined.

To add the reference, in your `article.json` file, inside your second `section` component, add a property named `style` with a value of `"bodyBackgroundStyle"`.

Your code should look like the example code Opaque Background: Result.

After you make these changes in your code, you can preview your working `article.json` file in News Preview to see that the lower section remains legible as it scrolls past the upper section.

#### Opaque Background: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "behavior": {
        "type": "parallax",
        "factor": 0.8
      },
      "components": [
        ...
      ]
    },
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "style": "bodyBackgroundStyle",
      "components": [
        ...
      ]
    }
  ],
  ...
}
```

### Previous

Creating a Layered Header

### Next

Viewing the Finished Article for Advanced Design Tutorial 1

## See Also

### Related Documentation

About Component Behaviors

Learn how to affect components’ reactions to device motion and scrolling.

object Parallax

The behavior whereby a component moves at a speed different from the scroll speed.

object ComponentStyle

The object for setting style properties for components, including background color and fill, borders, and table styles.

object Section

The component for organizing an article into sections.

### Advanced Design Tutorial 1: Headers and Parallax Behavior

Setting Up the Advanced Tutorials

Download the tutorial files, and learn about what you’ll create in the three advanced tutorials.

About Containers

Learn the basic Apple News Format container concepts required for the three advanced tutorials.

Creating a Layered Header

Create a header with a caption that’s layered in front of an image.

Viewing the Finished Article for Advanced Design Tutorial 1

See the full JSON code from this tutorial.

