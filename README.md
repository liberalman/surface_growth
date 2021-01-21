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

此时会生成一堆 .pdb 结尾的文件，想要查看这些文件，需要安装 VMD 软件，下载编译如下
```
wget http://www.ks.uiuc.edu/Research/vmd/vmd-1.9.3/files/final/vmd-1.9.3.bin.LINUXAMD64-CUDA8-OptiX4-OSPRay111p1.opengl.tar.gz
gunzip vmd-1.9.3.bin.LINUXAMD64-CUDA8-OptiX4-OSPRay111p1.opengl.tar.gz
tar -xvf vmd-1.9.3.bin.LINUXAMD64-CUDA8-OptiX4-OSPRay111p1.opengl.tar
cd vmd-1.9.3
./configure LINUXAMD64
./configure
cd src
sudo make install
```

安装完成后，用命令 vmd 启动即可，把 .pbd 文件加载进来，看看视觉效果。


