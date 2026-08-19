Sumber Belajar: https://www.youtube.com/watch?v=aTa7yj8AWqc&t=37s

Pastikan sudah download lalu install GNS3:
https://www.gns3.com/software/download
buat akun gns3, login dan download gns3.

Instalasi Mikrotik di Qemu
1. download file iso Mikrotik X86
2. buka CMD > Administrator
3. masuk folder C:\Program Files\GNS3\qemu-3.1.0
copykan iso mikrotik yang sudah di download
mikrotik-6.49.20.iso

4. buat harddisk qemu dengan perintah:
qemu-img.exe create -f qcow2 mikrotik.img 256M
Formatting 'mikrotik.img', fmt=qcow2 size=268435456 cluster_size=65536 lazy_refcounts=off refcount_bits=16

5. perintah install
qemu-system-x86_64.exe mikrotik.img -boot d -cdrom mikrotik-6.49.20.iso

6. menjalankan mikrotik di qemu
qemu-system-x86_64.exe mikrotik.img


