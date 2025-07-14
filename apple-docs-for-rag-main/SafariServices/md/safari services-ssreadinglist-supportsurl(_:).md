

- Safari Services
- SSReadingList
-  supportsURL(\_:) 

Type Method

# supportsURL(\_:)

Determines whether a URL can be added to the Reading List.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class func supportsURL(_ URL: URL) -> Bool
```

## Parameters 

`URL`  

The URL to be tested for Reading List support.

## Return Value

If true, then the URL is supported by Reading List; otherwise, false.

## Discussion

Use this method to determine whether to display a Reading List button in your app.

