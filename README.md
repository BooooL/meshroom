# ![Meshroom - 3D Reconstruction Sofware](/docs/logo/banner-meshroom.png)

Meshroom is a free, open-source 3D Reconstruction Software based on the [AliceVision](https://github.com/alicevision/AliceVision) framework.

Learn more details about the pipeline on [AliceVision website](http://alicevision.github.io).

See [results of the pipeline on sketchfab](http://sketchfab.com/AliceVision).


## Photogrammetry

Photogrammetry is the science of making measurements from photographs.
It infers the geometry of a scene from a set of unordered photographs or videos.
Photography is the projection of a 3D scene onto a 2D plane, losing depth information.
The goal of photogrammetry is to reverse this process.

See the [presentation of the pipeline steps](http://alicevision.github.io/#photogrammetry).


## License

The project is released under MPLv2, see [**COPYING.md**](COPYING.md).


## Get the project

See [**INSTALL.md**](INSTALL.md) to setup the project and pre-requisites.

Get the source code: `git clone --recursive git://github.com/alicevision/meshroom`

`cd meshroom`

Start Meshroom: `PYTHONPATH=$PWD python meshroom/ui`

On Ubuntu, you may have conflicts between native drivers and mesa drivers. In that case, you need to force usage of native drivers by adding them to the LD_LIBRARY_PATH:
`LD_LIBRARY_PATH=/usr/lib/nvidia-340 PYTHONPATH=$PWD python meshroom/ui`
You may need to adjust the folder `/usr/lib/nvidia-340` with the correct driver version.
