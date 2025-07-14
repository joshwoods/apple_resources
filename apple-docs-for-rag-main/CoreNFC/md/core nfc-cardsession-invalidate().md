

- Core NFC
- CardSession
-  invalidate() 

Instance Method

# invalidate()

Invalidates the current card emulation session.

iOS 17.4+iPadOS 17.4+

``` source
func invalidate()
```

## Discussion

This call stops any currently-running card emulation.

To restart, create a new CardSession instance with `startSession()`.

