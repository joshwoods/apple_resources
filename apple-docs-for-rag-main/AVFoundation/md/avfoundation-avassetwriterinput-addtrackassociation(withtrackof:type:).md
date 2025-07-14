

- AVFoundation
- AVAssetWriterInput
-  addTrackAssociation(withTrackOf:type:) 

Instance Method

# addTrackAssociation(withTrackOf:type:)

Adds an association between input tracks.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func addTrackAssociation(
    withTrackOf input: AVAssetWriterInput,
    type trackAssociationType: String
)
```

## Parameters 

`input`  

The input that contains the track to associate with this input’s track.

`trackAssociationType`  

The type of track association to add.

## Discussion

The system raises an error if the association type requires tracks of a media type that doesn’t match the input’s type, or if the output file type doesn’t support track associations.

You can’t add track associations after writing starts.

## See Also

### Configuring Track Associations

func canAddTrackAssociation(withTrackOf: AVAssetWriterInput, type: String) -> Bool

Determines whether it’s valid to associate another input’s track with this input’s track.

