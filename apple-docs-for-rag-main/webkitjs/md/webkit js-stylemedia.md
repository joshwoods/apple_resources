

- WebKit JS
-  StyleMedia 

Class

# StyleMedia

The `StyleMedia` class provides a way to evaluate CSS media queries from JavaScript. You do not need to, nor should you, create instances of this class. You access the shared `StyleMedia` object using the window’s styleMedia property.

Safari Desktop 10.0+Safari Mobile 4.2+

``` source
interface StyleMedia
```

## Overview

iOS Note

This class name changed from `Media` in iOS 4.2 and later.

## Topics

### Get Properties

type

A string that represents the media type of the current view used for rendering the document.

### Make Media Queries

matchMedium

Evaluates the given string as a media query and returns the result.

