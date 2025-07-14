

- Safari Services
- SFSafariExtensionHandling
-  contentBlocker(withIdentifier:blockedResourcesWith:on:) 

Instance Method

# contentBlocker(withIdentifier:blockedResourcesWith:on:)

Tells the handler which resources a content blocker blocked on a webpage.

macOS 10.15+

``` source
optional func contentBlocker(
    withIdentifier contentBlockerIdentifier: String,
    blockedResourcesWith urls: [URL],
    on page: SFSafariPage
)
```

## Parameters 

`contentBlockerIdentifier`  

The bundle identifier of the content blocker.

`urls`  

An array of URLs for the resources that the content blocker blocked.

`page`  

The webpage containing the resources that the content blocker blocked.

## Discussion

Safari calls this method when a content blocker associated with the extension performs a blocking action, and the extension has access to the URL that the content blocker blocked. The content blocker must be in the same containing app bundle as the extension.

To associate your content blocker with your extension, add an entry to your extension’s `Info.plist` file. Use the key `SFSafariAssociatedContentBlockers` and a value that’s an array of bundle identifiers for the content blockers.

