

- Core Graphics
- CGPath
-  intersection(\_:using:) 

Instance Method

# intersection(\_:using:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func intersection(
    _ other: CGPath,
    using rule: CGPathFillRule = .winding
) -> CGPath
```

## See Also

### Instance Methods

func applyWithBlock((UnsafePointer&lt;CGPathElement>) -> Void)

func componentsSeparated(using: CGPathFillRule) -> [CGPath]

func flattened(threshold: CGFloat) -> CGPath

func intersects(CGPath, using: CGPathFillRule) -> Bool

func lineIntersection(CGPath, using: CGPathFillRule) -> CGPath

func lineSubtracting(CGPath, using: CGPathFillRule) -> CGPath

func normalized(using: CGPathFillRule) -> CGPath

func subtracting(CGPath, using: CGPathFillRule) -> CGPath

func symmetricDifference(CGPath, using: CGPathFillRule) -> CGPath

func union(CGPath, using: CGPathFillRule) -> CGPath

