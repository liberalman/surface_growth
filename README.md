# surface_growth

install cuda
```sh
sudo apt install nvidia-cuda-toolkit
```

compile
```sh
nvcc -o bin/surface_growth surface_growth.cu surface_growth.cpp
```

run
```sh
cd bin
./surface_growth
```


