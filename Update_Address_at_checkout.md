PlaceSelectionViewController
```swift
fileprivate func didSelectPlace(_ poi: POI, locationType: LocationSearchType, reference: CLLocation?, metaInfo: GBPlaceSelectionMetaInfo?) {
  PlaceManager.sharedManager().saveSelectedPlace(poi.place)

  delegate?.didSelectPlace(poi, locationType: locationType, reference: reference, metaInfo: metaInfo)
}
```
