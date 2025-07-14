

- AVKit
- AVExperienceController
- AVExperienceController.Experiences
-  only(\_:) 

Type Method

# only(\_:)

Returns a set of experiences for the provided list.

visionOS 2.0+

``` source
static func only(_ experiences: C) -> AVExperienceController.Experiences where C : Collection, C.Element == AVExperienceController.Experience
```

## Parameters 

`experiences`  

The experiences to include. Order and duplication are not significant.

## Discussion

Use this method when the use case requires a specific set of experiences.

## See Also

### Defining experiences

static func recommended&lt;C>(excluding: C, including: C) -> AVExperienceController.Experiences

Returns the recommended set of experiences.

