

- Core Animation
-  CATransform3DInvert(\_:) 

Function

# CATransform3DInvert(\_:)

Inverts `t` and returns the result.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CATransform3DInvert(_ t: CATransform3D) -> CATransform3D
```

## Discussion

Returns the original matrix if `t` has no inverse.

