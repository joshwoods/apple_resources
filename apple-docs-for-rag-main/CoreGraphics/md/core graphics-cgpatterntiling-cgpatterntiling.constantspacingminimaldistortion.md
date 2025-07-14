

- Core Graphics
- CGPatternTiling
-  CGPatternTiling.constantSpacingMinimalDistortion 

Case

# CGPatternTiling.constantSpacingMinimalDistortion

Pattern cells are spaced consistently. Thepattern cell may be distorted by as much as 1 device pixel whenthe pattern is painted.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case constantSpacingMinimalDistortion
```

## See Also

### Constants

case noDistortion

The pattern cell is not distorted when painted.The spacing between pattern cells may vary by as much as 1 devicepixel.

case constantSpacing

Pattern cells are spaced consistently, as with CGPatternTiling.constantSpacingMinimalDistortion.The pattern cell may be distorted additionally to permit a moreefficient implementation.

