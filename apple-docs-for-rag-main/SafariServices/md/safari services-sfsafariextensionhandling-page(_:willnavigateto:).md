

- Safari Services
- SFSafariExtensionHandling
-  page(\_:willNavigateTo:) 

Instance Method

# page(\_:willNavigateTo:)

A method the system calls when a webpage is about to navigate to a new URL.

macOS 10.15+

``` source
optional func page(
    _ page: SFSafariPage,
    willNavigateTo url: URL?
)
```

## Parameters 

`page`  

The webpage from which the user or script initiated the navigation.

`url`  

A URL for the destination webpage.

## Discussion

The `url` parameter is `nil` if the extension does not have permission to access the destination webpage.

