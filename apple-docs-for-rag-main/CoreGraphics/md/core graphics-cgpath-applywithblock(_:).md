

- Core Graphics
- CGPath
-  applyWithBlock(\_:) 

Instance Method

# applyWithBlock(\_:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func applyWithBlock(_ block: (UnsafePointer) -> Void)
```

## See Also

### Instance Methods

func componentsSeparated(using: CGPathFillRule) -> [CGPath]

func flattened(threshold: CGFloat) -> CGPath

func intersection(CGPath, using: CGPathFillRule) -> CGPath

func intersects(CGPath, using: CGPathFillRule) -> Bool

func lineIntersection(CGPath, using: CGPathFillRule) -> CGPath

func lineSubtracting(CGPath, using: CGPathFillRule) -> CGPath

func normalized(using: CGPathFillRule) -> CGPath

func subtracting(CGPath, using: CGPathFillRule) -> CGPath

func symmetricDifference(CGPath, using: CGPathFillRule) -> CGPath

func union(CGPath, using: CGPathFillRule) -> CGPath

