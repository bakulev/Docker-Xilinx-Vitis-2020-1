# Docker-Xilinx-Vitis-2020-1
Docker container for Xilinx Vitis 2020.1

# docker-ubuntu-vivado
Dockerfile to create a Vivado 2020.1 installation under Ubuntu.
Modified from the 2019.2 version from <https://github.com/phwl/docker-vivado/tree/master/2020.1>.
Description is at <http://phwl.org/2020/xilinx-vivado-on-ubuntu-using-docker/>.

To build:

```bash
docker image build -t vivado-2020.1 .
```

To run:
```bash
docker run -e DISPLAY=`hostname`:0 -it --rm -v $PWD:/home/phwl/work -w /home/phwl vivado-2020.1
```
