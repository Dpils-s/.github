# Welcome to *Dpils-software!*

<p align="center">
<img src="https://github.com/Otrigos/Portfolio_S3_ArtjomsF/assets/92020227/9c70526e-55dc-41b0-a36f-83d1f461b088" alt="GIF Broke :(" width="50%" height="50%" />
</p>

*Dpils-s* is an open-source school project, providing delivery rider with a Rider-maps to get through their routes.

## Running the project

***

You will need local Mongo Database running.(You might use docker and docker image for mongoose)

First, you clone all of the following GIT repositories from this organization:

* Rider-maps
* Rider-Data
* Tick Service Discovery
* Tick Settings API

Unzip the files:

First open Rider-Data project in any preffered IDE.

Go to src/app.ts and change MongoDB connection string to your(usually it's done in .env file but my back-end for some reasons didn't want to work with it)

Then run in your Terminal from Rider-Data folder

```
npm i

npm run build

npm run start
```

If you succeed you should see something like this:

```
> rider-data@1.0.0 start
> node build/src/app.js

Connected to MongoDB!
App listening on port 4080!
```

Then open Rider-maps project

Then run in your Terminal from Rider-maps folder
```
npm i

npm run build

npm run serve
```
If you succeed you should see something like this:

```
> rider-system@0.1.0 serve
> vue-cli-service serve

 INFO  Starting development server...


 DONE  Compiled successfully in 1868ms                                                                                                                                                                                                                                                                    9:28:41 PM


  App running at:
  - Local:   http://localhost:4000/ 
  - Network: http://192.168.88.245:4000/

  Note that the development build is not optimized.
  To create a production build, run npm run build.

```

Then Front-end should be accesible with the link: http://localhost:4000/

There you will see navigation bar with only 2 links Home and Create Address

If you go to Create Address you will be redirected to a page where you can specify address(It's setted to show only addresses from Eindhoven and surroundings)
After you press "Save" button you should be redirected to Home page and see this address as in the list.
If you click "Start ride" button you will redirected to Route page where you will see the route(It sets routes for bikes and start point as imitation of Shop HUB is Fontys ICT building on Rachesmolen)

### That's it, I hope you enjoyed this small demo
