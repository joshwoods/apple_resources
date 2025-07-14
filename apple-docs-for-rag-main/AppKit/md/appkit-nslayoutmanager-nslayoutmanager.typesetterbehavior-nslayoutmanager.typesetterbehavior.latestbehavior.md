

- AppKit
- NSLayoutManager
- NSLayoutManager.TypesetterBehavior
-  NSLayoutManager.TypesetterBehavior.latestBehavior 

Case

# NSLayoutManager.TypesetterBehavior.latestBehavior

The current typesetter behavior in the current operating system.

macOS

``` source
case latestBehavior
```

## Discussion

For OS X v10.2, this behavior is identical to `NSTypesetterBehavior_10_2`. If you use this behavior setting, you cannot necessarily rely on line width and height metrics remaining the same across different versions of macOS.

## See Also

### Behaviors

case originalBehavior

The original typesetter behavior, as shipped with macOS 10.1 and earlier.

case behavior_10_2_WithCompatibility

The macOS 10.2 typesetting behavior that is still compatible with the original typesetter behavior.

case behavior_10_2

The typesetter behavior introduced in macOS 10.2.

case behavior_10_3

The typesetter behavior introduced in macOS 10.3.

case behavior_10_4

The typesetter behavior introduced in macOS 10.4.

