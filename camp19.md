# Fomu at CCCamp 2019

The workshop slides are available at [p.xobs.io/camp19](https://p.xobs.io/camp19/), and their source is at [github](https://git.xobs.io/xobs/cccamp-2019/)

In order to follow along with the Fomu workshop at CCCamp 2019, you will need the following materials, which should be available on a USB drive:

* Workshop Files
* Wishbone Tools
* dfu-util
* RISC-V compiler
* ICE40 FPGA toolchain
* Serial terminal program
* Python3

## Workshop Files

The workshop files are available on the USB drive, or in the [Fomu Workshop](https://github.com/im-fomu/fomu-workshop) repository.  You can clone them using git:

```sh
$ git clone https://github.com/im-fomu/fomu-workshop.git
```

Or [download a zipped version](https://github.com/im-fomu/fomu-workshop/archive/master.zip).

Pay special attention to [micropython-fomu.dfu](https://github.com/im-fomu/fomu-workshop/blob/master/micropython-fomu.dfu?raw=true), which will be used at the start of the class.


## Toolchain Files

The toolchain files should be provided on the USB drive that's being passed around.  However, you can download the files separately from [https://github.com/im-tomu/fomu-toolchain/releases](https://github.com/im-tomu/fomu-toolchain/releases).

## Raspberry Pi

Add the Fomu Raspbian repo:

```sh
$ sudo mount -oremount,rw /
$ echo 'deb https://repo.fomu.im/debian/ stretch main' | sudo tee /etc/apt/sources.list.d/fomu.list
$ wget -O - https://repo.fomu.im/tomu-signing-key.asc | sudo apt-key add -
```

Or manually get the packages from the [Fomu Repository](https://github.com/im-tomu/fomu-raspbian-packages/tree/master/debian/pool/main).

* riscv-toolchain
* yosys
* nextpnr-ice40
* icestorm
* picocom