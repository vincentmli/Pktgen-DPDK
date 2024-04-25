## Pktgen as lab DDoS tool

Record notes on how to custom pktgen to be used as DDoS
tool in lab.

## Build and Install

```
git clone https://github.com/vincentmli/Pktgen-DPDK.git

cd Pktgen-DPDK

meson build ( creates build directory under Pktgen-DPDK)

cd build

meson configure -Denable-avx2=false ( see https://github.com/pktgen/Pktgen-DPDK/issues/28)

ninja

ninja install
```
