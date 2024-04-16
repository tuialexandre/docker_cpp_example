## Dockerized build environment for C++



Docker based build environment example based on Dmitry Danilov's [post](https://ddanilov.me/dockerized-cpp-build)

### Buildind without docker

```
# Inside the project folder
mkdir build && cd build
cmake ..
make
```

### Building with docker
```
# Inside the project folder
make build-docker-deps-image
make
```

### Check executable
The executable should be inside the build folder and can be run with
```
./a.out
```