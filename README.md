# Google Api Python Web Client
Basic google api python client library. Get information on elevation data or use the directions api to view routes. Note, this project is still in development. If you want more information on googlemaps api's and python go here for [*googlemaps*](https://github.com/googlemaps/google-maps-services-python) module.

## Requirements
* Python >= 3.6
* urllib3 <= 1.25.8 
* Google developers console api key

## Contains
* Google Cloud Translate Api
* Google Elevation Api
* Google Directions Api
* Google Timezone Api
* Google Places Api

## Example
googleapi example using googleapi.places
```python
import googleapi

key = "Google api key"
place = googleapi.places(auth=key, place="Renwick Gallery of the Smithsonian American Art Museum, Washington")

#download image from photos.
placePhoto = place.photo(auth=key, download=True)
```
Downloaded image saved as "photoreference.jpg"
![photoreference](https://user-images.githubusercontent.com/57685626/76582781-9f1fc280-64ad-11ea-8c19-71f0f46e5a1a.jpg)
