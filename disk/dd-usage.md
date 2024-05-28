
- https://www.cyberciti.biz/faq/howto-linux-unix-test-disk-performance-with-dd-command/
- https://medium.com/azure-nigeria-community-group/benchmark-test-on-linux-virtual-machine-in-azure-d4dc59f1beeb
```
dd if=/dev/zero of=/tmp/test1.img bs=1G count=1 oflag=dsync
dd if=/dev/zero of=/tmp/test2.img bs=512 count=1000 oflag=dsync

diskspd –b8K –d30 –o4 –t8 –h –r –w25 –L –Z1G –c20G T:\iotest.dat > DiskSpeedResults.txt
sudo fio — directory=/data — name=randrw2.dat — ioengine=libaio — iodepth=64 — rw=randwrite — bs=4k — direct=1 — size=1024M
```