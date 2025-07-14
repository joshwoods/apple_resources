

- WebKit
- WebDataSource
-  unreachableURL Deprecated

Instance Property

# unreachableURL

The data source’s unreachable URL.

macOS 10.3–10.14Deprecated

``` source
var unreachableURL: URL! { get }
```

## Discussion

The data source has an unreachable URL if it was created using the \`\`WebFrame/loadAlternateHTMLString(\_:baseURL:forUnreachableURL:)\`\`\`WebFrame\` method.

