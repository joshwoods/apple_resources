

- Application Services
- ColorSync Manager
- Video Card Gamma Signatures
-  cmSigVideoCardGammaType 

Global Variable

# cmSigVideoCardGammaType

macOS 10.0+

``` source
var cmSigVideoCardGammaType: Int { get }
```

## Discussion

Constant that specifies video card gamma type signature in a video card gamma profile tag. That is, you use this constant to set the `typeDescriptor` field of the CMVideoCardGammaType structure. There is currently only one type possible for a video card gamma tag.

Starting with version 2.5, ColorSync supports an optional profile tag for video card gamma. The tag specifies gamma information, stored either as a formula or in table format, to be loaded into the video card when the profile containing the tag is put into use. As of version 2.5, the only ColorSync function that attempts to take advantage of video card gamma data is CMSetProfileByAVID.

