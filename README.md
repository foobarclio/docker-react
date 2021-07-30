`docker build -f Dockerfile.dev .` - `-f` use custom Dockerfile

`docker run -it -p 3000:3000 -v /app/node_modules -v $(pwd):/app IMAGE_ID`

`-it` - interactive

`-p 3000:3000` - mapping localhost ports : docker ports

`-v /app/node_modules` - exclude volume from syncronise with docker

`-v $(pwd):/app` - sync volume on $(pwd) path with folder `/app` on docker FS