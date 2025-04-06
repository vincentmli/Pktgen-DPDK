## Pktgen as lab DDoS tool

Record notes on how to custom pktgen to be used as DDoS
tool in lab.

## Build and Install

```
git clone https://github.com/vincentmli/Pktgen-DPDK.git

cd Pktgen-DPDK

git checkout vli-ddos

meson build ( creates build directory under Pktgen-DPDK)

cd build


#CPU that does not support avx2 and avx
(https://github.com/pktgen/Pktgen-DPDK/issues/28)
(https://github.com/pktgen/Pktgen-DPDK/issues/255)

meson configure -Denable-avx2=false -Denable-avx=false

ninja

ninja install
```
