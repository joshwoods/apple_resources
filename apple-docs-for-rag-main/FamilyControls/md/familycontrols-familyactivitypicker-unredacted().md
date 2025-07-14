

- FamilyControls
- FamilyActivityPicker
-  unredacted() 

Instance Method

# unredacted()

Removes any reason to apply a redaction to this view hierarchy.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func unredacted() -> some View
```

## See Also

### Privacy and Redaction

func privacySensitive(Bool) -> some View

Marks the view as containing sensitive, private user data.

func redacted(reason: RedactionReasons) -> some View

Adds a reason to apply a redaction to this view hierarchy.

