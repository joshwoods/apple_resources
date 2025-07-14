

- Apple News
- Apple News Format Tutorials
-  Adding a Scene 

Article

# Adding a Scene

Control how the article’s opening section comes into view.

## Overview

The fading sticky header scene causes the header to briefly “stick” to the top of the screen and then fade to a defined color.

**On this page, you’ll learn how to add a scene to your article.**

To implement a scene, you add a `scene` property to a `section` or `chapter` component.

### Apply a Scene

1.  In your working `article.json` file, delete the parallax behavior from the first section. The code you are deleting begins with `"behavior": {` and ends with a closing brace and a comma (`},`).

2.  Copy the example code Scene: Copy This Code.

3.  Paste the code inside the first section, replacing the behavior that you deleted in step 1.

Your code should look like the example code Scene: Result.

After you make this change in your code, you can preview your working `article.json` file in News Preview to see the fading sticky header scene.

#### Scene: Copy This Code

```
      "scene": {
        "type": "fading_sticky_header",
        "fadeColor": "#000"
      },
```

#### Scene: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "scene": {
        "type": "fading_sticky_header",
        "fadeColor": "#000"
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

### Previous

Adding Animations

### Next

Viewing the Finished Article for Advanced Design Tutorial 2

## See Also

### Related Documentation

Adding a Scene to a Chapter or a Section Header

Add a scene to your article to create special effects.

object FadingStickyHeader

The scene that briefly keeps a header at the top of the screen as the person scrolls through the article.

object Section

The component for organizing an article into sections.

### Advanced Design Tutorial 2: Layout and Positioning

Creating a Complex, Layered Header

Layer a title and heading in front of an image, with their colors optimized for legibility.

Creating a Floating Caption

Position a caption in the wide right margin of your article.

Creating an Inset Pull Quote

Wrap article body text around an inset pull quote.

Creating an Inset Photo

Wrap article body text around an inset photo.

Adding Color to Text Ranges

Create text in color by using HTML to refer to TextStyle objects.

Adding Animations

Use animations to affect how parts of your article come into view the first time they appear.

Viewing the Finished Article for Advanced Design Tutorial 2

See the full JSON code from this tutorial.

