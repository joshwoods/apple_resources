

- AVKit
- AVExperienceController
- AVExperienceController.Experiences
-  recommended(excluding:including:) 

Type Method

# recommended(excluding:including:)

Returns the recommended set of experiences.

visionOS 2.0+

``` source
static func recommended(
    excluding: C = [],
    including: C = []
) -> AVExperienceController.Experiences where C : Collection, C.Element == AVExperienceController.Experience
```

## Parameters 

`excluding`  

The experiences to remove. Removal happens before adding.

`including`  

The experiences to add. Redundant items are ignored.

## Discussion

Use this method to return the default recommended set of experiences for each platform and SDK version. Include or exclude experiences specifically desired or not supported by your app.

## See Also

### Defining experiences

static func only&lt;C>(C) -> AVExperienceController.Experiences

Returns a set of experiences for the provided list.

