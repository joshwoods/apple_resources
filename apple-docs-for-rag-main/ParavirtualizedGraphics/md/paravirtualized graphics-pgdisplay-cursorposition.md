

- Paravirtualized Graphics
- PGDisplay
-  cursorPosition 

Instance Property

# cursorPosition

The current cursor location in the guest environment.

Mac Catalyst 14.0+macOS 11.0+

``` source
var cursorPosition: PGDisplayCoord_t { get }
```

**Required**

## Discussion

If the cursor isn’t on the display, this property’s value is `(0xFFFF, 0xFFFF)`.

