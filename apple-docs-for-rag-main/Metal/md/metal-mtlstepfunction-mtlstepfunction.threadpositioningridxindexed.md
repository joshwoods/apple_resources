

- Metal
- MTLStepFunction
-  MTLStepFunction.threadPositionInGridXIndexed 

Case

# MTLStepFunction.threadPositionInGridXIndexed

The compute function fetches data by using the thread’s `x` coordinate to look up a value in the index buffer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case threadPositionInGridXIndexed
```

## Discussion

This step function uses the `x` coordinate of the thread position in a grid as an index into the `[[stage_in]]` index buffer, which is then used to fetch data. In tessellation compute kernels, you use this step function to identify a control point in a given patch.

## See Also

### Step options

case constant

The function fetches attribute data once.

case perInstance

The function fetches data based on the instance index.

case perPatch

The post-tessellation function fetches data based on the patch index of the patch.

case perPatchControlPoint

The post-tessellation function fetches data based on the control-point indices associated with the patch.

case perVertex

The vertex function fetches data for every vertex.

case threadPositionInGridX

The compute function fetches data based on the thread’s `x` coordinate.

case threadPositionInGridY

The compute function fetches data based on the thread’s `y` coordinate.

case threadPositionInGridYIndexed

The compute function fetches data by using the thread’s `y` coordinate to look up a value in the index buffer.

