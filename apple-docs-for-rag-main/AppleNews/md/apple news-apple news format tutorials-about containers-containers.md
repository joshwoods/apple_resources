

- Apple News
- Apple News Format Tutorials
-  About Containers 

Article

# About Containers

Learn the basic Apple News Format container concepts required for the three advanced tutorials.

## Overview

Most of the design and layout effects in this tutorial require you to create hierarchies of nested components. In Apple News Format JSON, a container is a component that can hold other components. Container components include four types: `chapter`, `header`, `section`, and `container`.

This is an example of a simple container.

```
```

In the example above, the `container` component has two child components. Notice that a container has a property named `components` whose value is an array. Any components inside the container’s `components` array are children of the container.

## See Also

### Related Documentation

Nesting Components in an Article

Use container components to create the component hierarchies you need for special article designs.

object Container

Properties shared by all container types.

### Advanced Design Tutorial 1: Headers and Parallax Behavior

Setting Up the Advanced Tutorials

Download the tutorial files, and learn about what you’ll create in the three advanced tutorials.

Creating a Layered Header

Create a header with a caption that’s layered in front of an image.

Adding Parallax Behavior

Create an illusion of multiple flat layers by causing the article body to overlap the header as the user scrolls.

Viewing the Finished Article for Advanced Design Tutorial 1

See the full JSON code from this tutorial.

