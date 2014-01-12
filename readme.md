# Leaflet for Meteor

[Leaflet.js](http://leafletjs.com/), a Javascript library for mobile-friendly interactive maps. 

## How to install 
1. npm install -g meteorite (if not already installed)
2. mrt add leaflet
3. edit the smart.json to reference the github repo
4. write the map code in Template.myTemplate.rendered
5. set in your client code the default image path 
6. enclose the map div in your template with the constant tag 

step 4
```javascript
  "packages": {
    "leaflet": {
      "git": "https://github.com/bevanhunt/leaflet",
      "branch": "master" 
    }
  }
```

step 5 
```javascript
L.Icon.Default.imagePath = 'packages/leaflet/images'
```

step 6
```html
{{#constant}}<div id="map">{{/constant}} 
```

## Plugins
If you want to add Leaflet plugins to your project - include them in your client folder - I prefer using the client/lib folder.

## GeoJSON 
I suggest the free web service - [Orge Web Service](http://ogre.adc4gis.com/) 

## Demo
Meteor Leafet Demo  |  [GitHub](https://github.com/bevanhunt/meteor-leaflet-demo)  |  [Demo](http://leaflet.meteor.com)

## License
MIT/X11
