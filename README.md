Openlayers 3 amd build
======================
Used for internal distribution.

The build is done with the new 'task' system in Openlayers: 
[doc](https://github.com/openlayers/ol3/tree/master/tasks)
([extra info](http://boundlessgeo.com/2014/10/openlayers-custom-builds-revisited/))

###install dependencies:
```
cd <project dir>
bower install
cd ol3
npm install
```

##how to build:
```
cd <project dir>/ol3
node tasks/build.js ../amd-build.json  ../ol.js
```

##how to release a new build:
+ Update ol3 using bower
+ Update the amd-build.json file
+ Create a new build
+ Copy the ol.css from ol3/css to the <project dir> folder if it has changed
+ Push to git
+ Run 'bower update ol3-amd' in projects using this dependency

##todo:
+ create separate build scripts for all projects, and set the "exports" parameter in each script with the correct list.