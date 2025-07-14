

- Kernel
- Kernel Constants
-  gOSKextUnresolved 

Global Variable

# gOSKextUnresolved

The value to which a kext's unresolved, weakly-referenced symbols are bound.

macOS 10.6+

``` source
const void *const gOSKextUnresolved;
```

## Discussion

A kext must test a weak symbol before using it. A weak symbol is only safe to use if it is not equal to `gOSKextUnresolved`.

Example for a weak symbol named `foo`:

      if (&amp;foo != gOSKextUnresolved) {
          foo();
      } else {
          printf(&quot;foo() is not supported\n&quot;);
      }

