### To use the image from scratch
1. [Generate the keystonejs project](http://keystonejs.com/getting-started/)
2. Optionally start [mongo db](https://hub.docker.com/_/mongo/)

        docker run --name mongo -d mongo
        docker run -p 27017:27017 --name mongo mongo

3. Add the mongo db settings into .env in keystonejs

        MONGO_URI=mongodb://mongo

4. Run the container by the following command

        docker run -p 80:3000 -it -d --link your-mongo:mongo --name keystonejs -v "$PWD":/usr/src/app ngyukman/keystonejs

