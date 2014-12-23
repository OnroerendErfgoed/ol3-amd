Openlayers 3 amd build
======================
Used for internal distribution.

The build is done with the new 'task' system in Openlayers: 
[doc](https://github.com/openlayers/ol3/tree/master/tasks)
([extra info](http://boundlessgeo.com/2014/10/openlayers-custom-builds-revisited/))

###install dependencies:
```
cd <project dir>
npm install
```

##how to build:
Custom build is no longer necessary, the build provided with openlayers 3.1.0 can be now used directly


##how to release a new build:
+ Update ol3 using npm
+ Copy ol.css from <project dir>/node_modules/openlayers/css/ to the <project dir> folder
+ Copy ol.js and ol-debug.js from <project dir>/node_modules/openlayers/dist/ to the <project dir> folder
+ Push to git
+ Run 'bower update ol3-amd' in the projects that use this dependency