

- MailKit
- MEExtension
-  handlerForContentBlocker() 

Instance Method

# handlerForContentBlocker()

Returns an object that provides rules that the message viewer uses to block content.

macOS 12.0+

``` source
@MainActor
optional func handlerForContentBlocker() -> any MEContentBlocker
```

## Return Value

An object that provides rules for blocking content.

