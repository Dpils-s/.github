# Welcome to *Dpils-software!*

<p align="center">
    <img src="https://github.com/Dpils-s/.github/assets/92020227/728611dc-7d1c-4b6d-8b0f-726b02693b11
"></img>
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

Then Front-end should be accesible with the link: http://localhost:4000/

There you will see navigation bar with only 2 links Home and Create Address

If you go to Create Address you will be redirected to a page where you can specify address(It's setted to show only addresses from Eindhoven and surroundings)
After you press "Save" button you should be redirected to Home page and see this address as in the list.
If you click "Start ride" button you will redirected to Route page where you will see the route(It sets routes for bikes and start point as imitation of Shop HUB is Fontys ICT building on Rachesmolen)

### That's it, I hope you enjoyed this small demo
