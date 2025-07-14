

- Apple News
- Apple News Format Tutorials
-  Creating a Sidebar 

Article

# Creating a Sidebar

Create a box with an HTML bulleted list in the margin.

## Overview

Placing supplemental or reference information in the margin of your article can create an informative and engaging experience.

**On this page, you’ll learn how to create a sidebar that contains some HTML formatting.**

### Create Component Layout Objects for the Sidebar

The `ComponentLayout` object called `sidebarLayout` specifies that the sidebar will begin in column 7 of the article layout and span three columns. The other `ComponentLayout` object makes a minor adjustment.

1.  Copy the example code Sidebar Layout Objects: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentLayout` object and the closing brace for the whole `componentLayouts` property.

Your code should look like the example code Sidebar Layout Objects: Result.

#### Sidebar Layout Objects: Copy This Code

```
,
    "sidebarLayout": {
      "contentInset": {
        "left": true,
        "right": true
      },
      "columnStart": 14,
      "columnSpan": 6,
      "margin": {
        "top": 24
      }
    },
    "fullMarginBelowContainedLayout": {
      "margin": {
        "bottom": 24
      }
    }
```

#### Sidebar Layout Objects: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentLayouts": {
    ...
    "sidebarLayout": {
      "contentInset": {
        "left": true,
        "right": true
      },
      "columnStart": 14,
      "columnSpan": 6,
      "margin": {
        "top": 24
      }
    },
    "fullMarginBelowContainedLayout": {
      "margin": {
        "bottom": 24
      }
    }
  },
  ...
}
```

### Define a Component Style Object for the Sidebar

Before you can apply a background color to the sidebar, you must define a new `ComponentStyle` object for the sidebar background color.

1.  Copy the example code sidebarBackgroundStyle: Copy This Code.

2.  Paste the code between the closing brace (`}`) of the last `ComponentStyle` object and the closing brace for the whole `componentStyles` property.

Your code should look like the example code sidebarBackgroundStyle: Result.

#### sidebarBackgroundStyle: Copy This Code

```
,
    "sidebarBackgroundStyle": {
      "backgroundColor": "#EAF1F4"
    }
```

#### sidebarBackgroundStyle: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "componentStyles": {
    ...
    "sidebarBackgroundStyle": {
      "backgroundColor": "#EAF1F4"
    }
  },
  ...
}
```

### Update the Body Component

In your working `article.json` file, update the `body` component that follows the `podcast` component.

1.  Copy the example code Body: Copy This Code.

2.  Paste the copied code, replacing the `body` component that follows the `podcast` component.

Your code should look like the example code Body: Result

#### Body: Copy This Code

```
{
  "identifier": "body2",
  "role": "body",
  "format": "html",
  "layout": "fullMarginAboveLayout",
  "text": "Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur? At vero eos et accusamus et iusto odio. Dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati.Sed dignissim magna nec metus tincidunt, in posuere tortor malesuada. Morbi auctor justo sodales nulla tincidunt rhoncus. Praesent aliquam, ex eu auctor auctor, turpis metus vehicula augue, non dapibus odio massa a massa. Nunc condimentum dui quis odio condimentum, ac sodales libero elementum. Nullam sagittis felis ac tortor varius ultricies. Duis aliquet ex vel orci aliquam, sit amet bibendum risus rhoncus. Interdum et malesuada fames ac ante ipsum primis in faucibus.Aliquam erat volutpat. Phasellus laoreet porttitor quam ut hendrerit. Aliquam nec arcu scelerisque, scelerisque nisi sit amet, eleifend augue. Nunc sit amet elit commodo, congue felis eget, gravida nibh. Praesent lorem risus, tristique sed porta non, aliquam in sapien. Praesent rhoncus orci eu scelerisque euismod. Morbi bibendum lorem lorem, eu tincidunt neque volutpat sit amet. Sed urna ligula, volutpat nec posuere a, laoreet ut tellus. Curabitur lacinia ornare nisi, et aliquet ex pretium sit amet. Aliquam finibus tristique arcu at feugiat. Donec nec sodales magna. Nulla vulputate sem eget libero venenatis lobortis. Morbi nec sodales metus. Ut eu diam quis augue imperdiet interdum ac quis metus."
},
```

#### Body: Result

Ellipses (`...`) indicate lines of code that have been omitted from this example.

```
{
  ...
  "components": [
    ...
    {
      "role": "section",
      "layout": "fullBleedLayout",
      "style": "bodyBackgroundStyle",
      "components": [
        ...
        {
          "role": "podcast",
          "layout": "noMarginLayout",
          "orientation": "horizontal",
          "URL": "https://podcasts.apple.com/us/podcast/apple-news-today/id1473872585"
        },
        {
          "identifier": "body2",
          "role": "body",
          "format": "html",
          "layout": "fullMarginAboveLayout",
          "text": "Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur? At vero eos et accusamus et iusto odio. Dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati.Sed dignissim magna nec metus tincidunt, in posuere tortor malesuada. Morbi auctor justo sodales nulla tincidunt rhoncus. Praesent aliquam, ex eu auctor auctor, turpis metus vehicula augue, non dapibus odio massa a massa. Nunc condimentum dui quis odio condimentum, ac sodales libero elementum. Nullam sagittis felis ac tortor varius ultricies. Duis aliquet ex vel orci aliquam, sit amet bibendum risus rhoncus. Interdum et malesuada fames ac ante ipsum primis in faucibus.Aliquam erat volutpat. Phasellus laoreet porttitor quam ut hendrerit. Aliquam nec arcu scelerisque, scelerisque nisi sit amet, eleifend augue. Nunc sit amet elit commodo, congue felis eget, gravida nibh. Praesent lorem risus, tristique sed porta non, aliquam in sapien. Praesent rhoncus orci eu scelerisque euismod. Morbi bibendum lorem lorem, eu tincidunt neque volutpat sit amet. Sed urna ligula, volutpat nec posuere a, laoreet ut tellus. Curabitur lacinia ornare nisi, et aliquet ex pretium sit amet. Aliquam finibus tristique arcu at feugiat. Donec nec sodales magna. Nulla vulputate sem eget libero venenatis lobortis. Morbi nec sodales metus. Ut eu diam quis augue imperdiet interdum ac quis metus."
        },
        ...
      ]
    }
  ],
  ...
}
```

### Add and Anchor the Sidebar Content

In your working `article.json` file, the `body` component that follows the `podcast` component should now have an `identifier` property with the value `body2`.

1.  Copy the example code Container: Copy This Code.

2.  Paste the code after the closing brace and comma at the end of the body component that contains an identifier property with the value `body2`.

Your code should look like the example code Container: Result.

#### Container: Copy This Code

```
{
  "role": "container",
  "layout": "sidebarLayout",
  "style": "sidebarBackgroundStyle",
  "anchor": {
    "targetComponentIdentifier": "body2",
    "targetAnchorPosition": "bottom",
    "originAnchorPosition": "bottom"
  },
  "animation": {
    "type": "fade_in",
    "userControllable": true,
    "initialAlpha": 0.5
  },
  "components": [
    {
      "role": "heading3",
      "layout": "halfMarginBothContainedLayout",
      "text": "EPISODES OF NOTE"
    },
    {
      "role": "divider",
      "layout": "halfMarginBelowContainedLayout",
      "stroke": {
        "width": 1,
        "color": "#A6AAA9"
      }
    },
    {
      "role": "caption",
      "layout": "fullMarginBelowContainedLayout",
      "format": "html",
      "text": " At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis. Praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi. Sint occaecati cupiditate non provident. similique sunt in culpa qui officia deserunt mollitia animi. Et harum quidem rerum facilis est et expedita distinctio."
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
      "layout": "fullBleedLayout",
      "style": "bodyBackgroundStyle",
      "components": [
        ...
        {
          "identifier": "body2",
          "role": "body",
          "format": "html",
          "layout": "fullMarginAboveLayout",
          "text": "Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur? At vero eos et accusamus et iusto odio. Dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati.Sed dignissim magna nec metus tincidunt, in posuere tortor malesuada. Morbi auctor justo sodales nulla tincidunt rhoncus. Praesent aliquam, ex eu auctor auctor, turpis metus vehicula augue, non dapibus odio massa a massa. Nunc condimentum dui quis odio condimentum, ac sodales libero elementum. Nullam sagittis felis ac tortor varius ultricies. Duis aliquet ex vel orci aliquam, sit amet bibendum risus rhoncus. Interdum et malesuada fames ac ante ipsum primis in faucibus.Aliquam erat volutpat. Phasellus laoreet porttitor quam ut hendrerit. Aliquam nec arcu scelerisque, scelerisque nisi sit amet, eleifend augue. Nunc sit amet elit commodo, congue felis eget, gravida nibh. Praesent lorem risus, tristique sed porta non, aliquam in sapien. Praesent rhoncus orci eu scelerisque euismod. Morbi bibendum lorem lorem, eu tincidunt neque volutpat sit amet. Sed urna ligula, volutpat nec posuere a, laoreet ut tellus. Curabitur lacinia ornare nisi, et aliquet ex pretium sit amet. Aliquam finibus tristique arcu at feugiat. Donec nec sodales magna. Nulla vulputate sem eget libero venenatis lobortis. Morbi nec sodales metus. Ut eu diam quis augue imperdiet interdum ac quis metus."
        },
        {
          "role": "container",
          "layout": "sidebarLayout",
          "style": "sidebarBackgroundStyle",
          "anchor": {
            "targetComponentIdentifier": "body2",
            "targetAnchorPosition": "bottom",
            "originAnchorPosition": "bottom"
          },
          "animation": {
            "type": "fade_in",
            "userControllable": true,
            "initialAlpha": 0.5
          },
          "components": [
            {
              "role": "heading3",
              "layout": "halfMarginBothContainedLayout",
              "text": "EPISODES OF NOTE"
            },
            {
              "role": "divider",
              "layout": "halfMarginBelowContainedLayout",
              "stroke": {
                "width": 1,
                "color": "#A6AAA9"
              }
            },
            {
              "role": "caption",
              "layout": "fullMarginBelowContainedLayout",
              "format": "html",
              "text": " At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis. Praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi. Sint occaecati cupiditate non provident. similique sunt in culpa qui officia deserunt mollitia animi. Et harum quidem rerum facilis est et expedita distinctio."
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

### Previous

Adding a Video

### Next

Adding a Fixed Image Fill

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

object Anchor

The object for anchoring one component to another component in your article’s layout.

Using HTML with Apple News Format

Use HTML formatting for text components.

### Advanced Design Tutorial 3: More Ideas

Giving the Article a Dark Color Scheme

Apply a new color scheme to your article.

Adding a Video

Add a video component inside the header component.

Adding a Fixed Image Fill

Add an image that remains stationary when the user scrolls.

Creating a Newsletter Sign-Up Element

Add a newsletter sign-up element in your article.

Viewing the Finished Article for Advanced Design Tutorial 3

See the full JSON code from this tutorial.

