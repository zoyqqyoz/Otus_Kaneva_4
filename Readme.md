ДЗ 4: Стенд с Vagrant c ZFS

1. Поднимаем ВМ из Vagrantfile с предустановленной zfs
```
Bringing machine 'zfs' up with 'virtualbox' provider...
==> zfs: Box 'centos/7' could not be found. Attempting to find and install...
    zfs: Box Provider: virtualbox
    zfs: Box Version: 2004.01
==> zfs: Loading metadata for box 'centos/7'
    zfs: URL: https://vagrantcloud.com/centos/7
==> zfs: Adding box 'centos/7' (v2004.01) for provider: virtualbox
    zfs: Downloading: https://vagrantcloud.com/centos/boxes/7/versions/2004.01/providers/virtualbox.box

Progress: 0% (Rate: 0*/s, Estimated time remaining: --:--:--)
Progress: 100% (Rate: 317/s, Estimated time remaining: --:--:--)
Download redirected to host: cloud.centos.org

Progress: 100% (Rate: 148/s, Estimated time remaining: --:--:--)
Progress: 0% (Rate: 0*/s, Estimated time remaining: --:--:--)
Progress: 0% (Rate: 2309k*/s, Estimated time remaining: 0:07:32)
Progress: 1% (Rate: 2772k*/s, Estimated time remaining: 0:04:30)
Progress: 1% (Rate: 3038k*/s, Estimated time remaining: 0:03:33)
Progress: 2% (Rate: 3225k*/s, Estimated time remaining: 0:03:04)
Progress: 3% (Rate: 3385k*/s, Estimated time remaining: 0:02:46)
Progress: 4% (Rate: 3629k*/s, Estimated time remaining: 0:02:38)
Progress: 5% (Rate: 3727k*/s, Estimated time remaining: 0:02:31)
Progress: 6% (Rate: 3840k*/s, Estimated time remaining: 0:02:23)
Progress: 6% (Rate: 3810k*/s, Estimated time remaining: 0:02:19)
Progress: 7% (Rate: 3645k*/s, Estimated time remaining: 0:02:18)
Progress: 7% (Rate: 3331k*/s, Estimated time remaining: 0:02:22)
Progress: 8% (Rate: 3018k*/s, Estimated time remaining: 0:02:24)
Progress: 8% (Rate: 2677k*/s, Estimated time remaining: 0:02:25)
Progress: 9% (Rate: 2498k*/s, Estimated time remaining: 0:02:25)
Progress: 10% (Rate: 2465k*/s, Estimated time remaining: 0:02:23)
Progress: 10% (Rate: 2725k*/s, Estimated time remaining: 0:02:21)
Progress: 11% (Rate: 3009k*/s, Estimated time remaining: 0:02:18)
Progress: 12% (Rate: 3169k*/s, Estimated time remaining: 0:02:17)
Progress: 13% (Rate: 3293k*/s, Estimated time remaining: 0:02:15)
Progress: 13% (Rate: 3411k*/s, Estimated time remaining: 0:02:12)
Progress: 14% (Rate: 3387k*/s, Estimated time remaining: 0:02:11)
Progress: 15% (Rate: 3279k*/s, Estimated time remaining: 0:02:10)
Progress: 15% (Rate: 3296k*/s, Estimated time remaining: 0:02:08)
Progress: 16% (Rate: 3340k*/s, Estimated time remaining: 0:02:06)
Progress: 17% (Rate: 3364k*/s, Estimated time remaining: 0:02:04)
Progress: 18% (Rate: 3529k*/s, Estimated time remaining: 0:02:02)
Progress: 18% (Rate: 3588k*/s, Estimated time remaining: 0:02:00)
Progress: 19% (Rate: 3699k*/s, Estimated time remaining: 0:01:58)
Progress: 20% (Rate: 3675k*/s, Estimated time remaining: 0:01:57)
Progress: 21% (Rate: 3557k*/s, Estimated time remaining: 0:01:56)
Progress: 21% (Rate: 3461k*/s, Estimated time remaining: 0:01:54)
Progress: 22% (Rate: 3540k*/s, Estimated time remaining: 0:01:52)
Progress: 23% (Rate: 3565k*/s, Estimated time remaining: 0:01:50)
Progress: 24% (Rate: 3634k*/s, Estimated time remaining: 0:01:49)
Progress: 25% (Rate: 3716k*/s, Estimated time remaining: 0:01:47)
Progress: 26% (Rate: 3810k*/s, Estimated time remaining: 0:01:45)
Progress: 26% (Rate: 3889k*/s, Estimated time remaining: 0:01:43)
Progress: 27% (Rate: 3820k*/s, Estimated time remaining: 0:01:42)
Progress: 28% (Rate: 3778k*/s, Estimated time remaining: 0:01:41)
Progress: 29% (Rate: 3650k*/s, Estimated time remaining: 0:01:40)
Progress: 29% (Rate: 3360k*/s, Estimated time remaining: 0:01:40)
Progress: 30% (Rate: 3044k*/s, Estimated time remaining: 0:01:40)
Progress: 30% (Rate: 2881k*/s, Estimated time remaining: 0:01:39)
Progress: 31% (Rate: 2786k*/s, Estimated time remaining: 0:01:38)
Progress: 32% (Rate: 2868k*/s, Estimated time remaining: 0:01:37)
Progress: 32% (Rate: 3100k*/s, Estimated time remaining: 0:01:36)
Progress: 33% (Rate: 3391k*/s, Estimated time remaining: 0:01:34)
Progress: 34% (Rate: 3656k*/s, Estimated time remaining: 0:01:32)
Progress: 35% (Rate: 3749k*/s, Estimated time remaining: 0:01:31)
Progress: 36% (Rate: 3858k*/s, Estimated time remaining: 0:01:30)
Progress: 37% (Rate: 3956k*/s, Estimated time remaining: 0:01:28)
Progress: 38% (Rate: 3910k*/s, Estimated time remaining: 0:01:27)
Progress: 38% (Rate: 3482k*/s, Estimated time remaining: 0:01:27)
Progress: 38% (Rate: 3057k*/s, Estimated time remaining: 0:01:27)
Progress: 39% (Rate: 2627k*/s, Estimated time remaining: 0:01:27)
Progress: 39% (Rate: 2199k*/s, Estimated time remaining: 0:01:27)
Progress: 40% (Rate: 1913k*/s, Estimated time remaining: 0:01:27)
Progress: 40% (Rate: 2032k*/s, Estimated time remaining: 0:01:26)
Progress: 41% (Rate: 2307k*/s, Estimated time remaining: 0:01:26)
Progress: 41% (Rate: 2607k*/s, Estimated time remaining: 0:01:25)
Progress: 42% (Rate: 2910k*/s, Estimated time remaining: 0:01:23)
Progress: 43% (Rate: 3238k*/s, Estimated time remaining: 0:01:22)
Progress: 44% (Rate: 3770k*/s, Estimated time remaining: 0:01:19)
Progress: 45% (Rate: 4167k*/s, Estimated time remaining: 0:01:17)
Progress: 46% (Rate: 4256k*/s, Estimated time remaining: 0:01:16)
Progress: 47% (Rate: 4146k*/s, Estimated time remaining: 0:01:15)
Progress: 47% (Rate: 3985k*/s, Estimated time remaining: 0:01:14)
Progress: 48% (Rate: 3475k*/s, Estimated time remaining: 0:01:14)
Progress: 49% (Rate: 3125k*/s, Estimated time remaining: 0:01:13)
Progress: 49% (Rate: 3023k*/s, Estimated time remaining: 0:01:12)
Progress: 50% (Rate: 3101k*/s, Estimated time remaining: 0:01:11)
Progress: 51% (Rate: 3188k*/s, Estimated time remaining: 0:01:09)
Progress: 52% (Rate: 3419k*/s, Estimated time remaining: 0:01:08)
Progress: 52% (Rate: 3637k*/s, Estimated time remaining: 0:01:07)
Progress: 53% (Rate: 3886k*/s, Estimated time remaining: 0:01:05)
Progress: 54% (Rate: 4007k*/s, Estimated time remaining: 0:01:04)
Progress: 55% (Rate: 4047k*/s, Estimated time remaining: 0:01:02)
Progress: 56% (Rate: 4038k*/s, Estimated time remaining: 0:01:01)
Progress: 57% (Rate: 3888k*/s, Estimated time remaining: 0:01:00)
Progress: 57% (Rate: 3593k*/s, Estimated time remaining: 0:00:59)
Progress: 58% (Rate: 3360k*/s, Estimated time remaining: 0:00:58)
Progress: 59% (Rate: 3240k*/s, Estimated time remaining: 0:00:58)
Progress: 59% (Rate: 3169k*/s, Estimated time remaining: 0:00:56)
Progress: 60% (Rate: 3242k*/s, Estimated time remaining: 0:00:55)
Progress: 61% (Rate: 3393k*/s, Estimated time remaining: 0:00:54)
Progress: 62% (Rate: 3455k*/s, Estimated time remaining: 0:00:53)
Progress: 62% (Rate: 3156k*/s, Estimated time remaining: 0:00:53)
Progress: 62% (Rate: 2645k*/s, Estimated time remaining: 0:00:53)
Progress: 62% (Rate: 1997k*/s, Estimated time remaining: 0:00:53)
Progress: 62% (Rate: 1360k*/s, Estimated time remaining: 0:00:54)
Progress: 63% (Rate: 896k*/s, Estimated time remaining: 0:00:54)
Progress: 63% (Rate: 773k*/s, Estimated time remaining: 0:00:54)
Progress: 63% (Rate: 875k*/s, Estimated time remaining: 0:00:54)
Progress: 63% (Rate: 1113k*/s, Estimated time remaining: 0:00:54)
Progress: 64% (Rate: 1409k*/s, Estimated time remaining: 0:00:53)
Progress: 64% (Rate: 1697k*/s, Estimated time remaining: 0:00:53)
Progress: 65% (Rate: 1922k*/s, Estimated time remaining: 0:00:52)
Progress: 65% (Rate: 2107k*/s, Estimated time remaining: 0:00:51)
Progress: 66% (Rate: 2267k*/s, Estimated time remaining: 0:00:51)
Progress: 66% (Rate: 2409k*/s, Estimated time remaining: 0:00:50)
Progress: 67% (Rate: 2568k*/s, Estimated time remaining: 0:00:49)
Progress: 68% (Rate: 2778k*/s, Estimated time remaining: 0:00:48)
Progress: 69% (Rate: 3021k*/s, Estimated time remaining: 0:00:46)
Progress: 69% (Rate: 3305k*/s, Estimated time remaining: 0:00:45)
Progress: 70% (Rate: 3553k*/s, Estimated time remaining: 0:00:44)
Progress: 71% (Rate: 3658k*/s, Estimated time remaining: 0:00:42)
Progress: 72% (Rate: 3681k*/s, Estimated time remaining: 0:00:41)
Progress: 72% (Rate: 3577k*/s, Estimated time remaining: 0:00:40)
Progress: 73% (Rate: 3335k*/s, Estimated time remaining: 0:00:40)
Progress: 73% (Rate: 3049k*/s, Estimated time remaining: 0:00:39)
Progress: 74% (Rate: 2902k*/s, Estimated time remaining: 0:00:38)
Progress: 75% (Rate: 2798k*/s, Estimated time remaining: 0:00:37)
Progress: 75% (Rate: 2653k*/s, Estimated time remaining: 0:00:36)
Progress: 76% (Rate: 2445k*/s, Estimated time remaining: 0:00:36)
Progress: 76% (Rate: 2276k*/s, Estimated time remaining: 0:00:36)
Progress: 76% (Rate: 2120k*/s, Estimated time remaining: 0:00:35)
Progress: 77% (Rate: 2011k*/s, Estimated time remaining: 0:00:34)
Progress: 77% (Rate: 2071k*/s, Estimated time remaining: 0:00:34)
Progress: 78% (Rate: 2321k*/s, Estimated time remaining: 0:00:33)
Progress: 79% (Rate: 2607k*/s, Estimated time remaining: 0:00:32)
Progress: 79% (Rate: 2875k*/s, Estimated time remaining: 0:00:30)
Progress: 80% (Rate: 2990k*/s, Estimated time remaining: 0:00:29)
Progress: 81% (Rate: 3139k*/s, Estimated time remaining: 0:00:28)
Progress: 82% (Rate: 3254k*/s, Estimated time remaining: 0:00:27)
Progress: 82% (Rate: 3162k*/s, Estimated time remaining: 0:00:26)
Progress: 83% (Rate: 2928k*/s, Estimated time remaining: 0:00:26)
Progress: 83% (Rate: 2847k*/s, Estimated time remaining: 0:00:25)
Progress: 84% (Rate: 2720k*/s, Estimated time remaining: 0:00:24)
Progress: 84% (Rate: 2493k*/s, Estimated time remaining: 0:00:23)
Progress: 85% (Rate: 2243k*/s, Estimated time remaining: 0:00:23)
Progress: 85% (Rate: 2113k*/s, Estimated time remaining: 0:00:22)
Progress: 85% (Rate: 1990k*/s, Estimated time remaining: 0:00:22)
Progress: 86% (Rate: 1813k*/s, Estimated time remaining: 0:00:21)
Progress: 86% (Rate: 1710k*/s, Estimated time remaining: 0:00:21)
Progress: 87% (Rate: 1844k*/s, Estimated time remaining: 0:00:20)
Progress: 87% (Rate: 1991k*/s, Estimated time remaining: 0:00:19)
Progress: 88% (Rate: 2138k*/s, Estimated time remaining: 0:00:19)
Progress: 88% (Rate: 2221k*/s, Estimated time remaining: 0:00:18)
Progress: 88% (Rate: 2037k*/s, Estimated time remaining: 0:00:18)
Progress: 88% (Rate: 1831k*/s, Estimated time remaining: 0:00:17)
Progress: 89% (Rate: 1638k*/s, Estimated time remaining: 0:00:17)
Progress: 89% (Rate: 1445k*/s, Estimated time remaining: 0:00:16)
Progress: 90% (Rate: 1387k*/s, Estimated time remaining: 0:00:16)
Progress: 90% (Rate: 1647k*/s, Estimated time remaining: 0:00:15)
Progress: 91% (Rate: 1934k*/s, Estimated time remaining: 0:00:14)
Progress: 91% (Rate: 1989k*/s, Estimated time remaining: 0:00:14)
Progress: 91% (Rate: 1994k*/s, Estimated time remaining: 0:00:13)
Progress: 92% (Rate: 2009k*/s, Estimated time remaining: 0:00:12)
Progress: 92% (Rate: 1945k*/s, Estimated time remaining: 0:00:12)
Progress: 93% (Rate: 1840k*/s, Estimated time remaining: 0:00:11)
Progress: 93% (Rate: 1853k*/s, Estimated time remaining: 0:00:11)
Progress: 93% (Rate: 1886k*/s, Estimated time remaining: 0:00:10)
Progress: 94% (Rate: 1914k*/s, Estimated time remaining: 0:00:09)
Progress: 94% (Rate: 1999k*/s, Estimated time remaining: 0:00:08)
Progress: 95% (Rate: 2023k*/s, Estimated time remaining: 0:00:08)
Progress: 95% (Rate: 2167k*/s, Estimated time remaining: 0:00:07)
Progress: 96% (Rate: 2318k*/s, Estimated time remaining: 0:00:06)
Progress: 96% (Rate: 2463k*/s, Estimated time remaining: 0:00:05)
Progress: 97% (Rate: 2611k*/s, Estimated time remaining: 0:00:04)
Progress: 98% (Rate: 2866k*/s, Estimated time remaining: 0:00:03)
Progress: 99% (Rate: 3125k*/s, Estimated time remaining: 0:00:01)
Progress: 99% (Rate: 3214k*/s, Estimated time remaining: --:--:--)
    zfs: Calculating and comparing box checksum...
==> zfs: Successfully added box 'centos/7' (v2004.01) for 'virtualbox'!
==> zfs: Importing base box 'centos/7'...

Progress: 20%
Progress: 40%
Progress: 70%
Progress: 90%
==> zfs: Matching MAC address for NAT networking...
==> zfs: Checking if box 'centos/7' version '2004.01' is up to date...
==> zfs: Setting the name of the VM: neva_zfs_1684824364762_55658
==> zfs: Fixed port collision for 22 => 2222. Now on port 2200.
==> zfs: Clearing any previously set network interfaces...
==> zfs: Preparing network interfaces based on configuration...
    zfs: Adapter 1: nat
==> zfs: Forwarding ports...
    zfs: 22 (guest) => 2200 (host) (adapter 1)
==> zfs: Running 'pre-boot' VM customizations...
==> zfs: Booting VM...
==> zfs: Waiting for machine to boot. This may take a few minutes...
    zfs: SSH address: 127.0.0.1:2200
    zfs: SSH username: vagrant
    zfs: SSH auth method: private key
    zfs: 
    zfs: Vagrant insecure key detected. Vagrant will automatically replace
    zfs: this with a newly generated keypair for better security.
    zfs: 
    zfs: Inserting generated public key within guest...
    zfs: Removing insecure key from the guest if it's present...
    zfs: Key inserted! Disconnecting and reconnecting using new SSH key...
==> zfs: Machine booted and ready!
==> zfs: Checking for guest additions in VM...
    zfs: No guest additions were detected on the base box for this VM! Guest
    zfs: additions are required for forwarded ports, shared folders, host only
    zfs: networking, and more. If SSH fails on this machine, please install
    zfs: the guest additions and repackage the box to continue.
    zfs: 
    zfs: This is not an error message; everything may continue to work properly,
    zfs: in which case you may ignore this message.
==> zfs: Setting hostname...
==> zfs: Running provisioner: shell...
    zfs: Running: inline script
    zfs: Loaded plugins: fastestmirror
    zfs: Examining /var/tmp/yum-root-x2cldZ/zfs-release.el7_8.noarch.rpm: zfs-release-1-7.8.noarch
    zfs: Marking /var/tmp/yum-root-x2cldZ/zfs-release.el7_8.noarch.rpm to be installed
    zfs: Resolving Dependencies
    zfs: --> Running transaction check
    zfs: ---> Package zfs-release.noarch 0:1-7.8 will be installed
    zfs: --> Finished Dependency Resolution
    zfs: 
    zfs: Dependencies Resolved
    zfs: 
    zfs: ================================================================================
    zfs:  Package          Arch        Version      Repository                      Size
    zfs: ================================================================================
    zfs: Installing:
    zfs:  zfs-release      noarch      1-7.8        /zfs-release.el7_8.noarch      2.9 k
    zfs: 
    zfs: Transaction Summary
    zfs: ================================================================================
    zfs: Install  1 Package
    zfs: 
    zfs: Total size: 2.9 k
    zfs: Installed size: 2.9 k
    zfs: Downloading packages:
    zfs: Running transaction check
    zfs: Running transaction test
    zfs: Transaction test succeeded
    zfs: Running transaction
    zfs:   Installing : zfs-release-1-7.8.noarch                                     1/1
    zfs:   Verifying  : zfs-release-1-7.8.noarch                                     1/1
    zfs: 
    zfs: Installed:
    zfs:   zfs-release.noarch 0:1-7.8
    zfs: 
    zfs: Complete!
    zfs: Loaded plugins: fastestmirror
    zfs: Determining fastest mirrors
    zfs:  * base: mirror.23m.com
    zfs:  * extras: ftp.plusline.net
    zfs:  * updates: mirror.23m.com
    zfs: Resolving Dependencies
    zfs: --> Running transaction check
    zfs: ---> Package epel-release.noarch 0:7-11 will be installed
    zfs: ---> Package kernel-devel.x86_64 0:3.10.0-1160.90.1.el7 will be installed
    zfs: --> Processing Dependency: perl for package: kernel-devel-3.10.0-1160.90.1.el7.x86_64
    zfs: ---> Package zfs.x86_64 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: zfs-kmod = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzpool2 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzfs2 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libuutil1 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libnvpair1 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: sysstat for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzpool.so.2()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzfs_core.so.1()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzfs.so.2()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libuutil.so.1()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libnvpair.so.1()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Running transaction check
    zfs: ---> Package libnvpair1.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libuutil1.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libzfs2.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libzpool2.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package perl.x86_64 4:5.16.3-299.el7_9 will be installed
    zfs: --> Processing Dependency: perl-libs = 4:5.16.3-299.el7_9 for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Socket) >= 1.3 for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Scalar::Util) >= 1.10 for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl-macros for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl-libs for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(threads::shared) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(threads) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(constant) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Time::Local) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Time::HiRes) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Storable) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Socket) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Scalar::Util) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Pod::Simple::XHTML) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Pod::Simple::Search) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Getopt::Long) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Filter::Util::Call) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(File::Temp) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(File::Spec::Unix) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(File::Spec::Functions) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(File::Spec) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(File::Path) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Exporter) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Cwd) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: perl(Carp) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: --> Processing Dependency: libperl.so()(64bit) for package: 4:perl-5.16.3-299.el7_9.x86_64
    zfs: ---> Package sysstat.x86_64 0:10.1.5-20.el7_9 will be installed
    zfs: --> Processing Dependency: libsensors.so.4()(64bit) for package: sysstat-10.1.5-20.el7_9.x86_64
    zfs: ---> Package zfs-dkms.noarch 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: dkms >= 2.2.0.3 for package: zfs-dkms-0.8.5-1.el7.noarch
    zfs: --> Processing Dependency: gcc for package: zfs-dkms-0.8.5-1.el7.noarch
    zfs: --> Running transaction check
    zfs: ---> Package gcc.x86_64 0:4.8.5-44.el7 will be installed
    zfs: --> Processing Dependency: libgomp = 4.8.5-44.el7 for package: gcc-4.8.5-44.el7.x86_64
    zfs: --> Processing Dependency: cpp = 4.8.5-44.el7 for package: gcc-4.8.5-44.el7.x86_64
    zfs: --> Processing Dependency: libgcc >= 4.8.5-44.el7 for package: gcc-4.8.5-44.el7.x86_64
    zfs: --> Processing Dependency: glibc-devel >= 2.2.90-12 for package: gcc-4.8.5-44.el7.x86_64
    zfs: --> Processing Dependency: libmpfr.so.4()(64bit) for package: gcc-4.8.5-44.el7.x86_64
    zfs: --> Processing Dependency: libmpc.so.3()(64bit) for package: gcc-4.8.5-44.el7.x86_64
    zfs: ---> Package lm_sensors-libs.x86_64 0:3.4.0-8.20160601gitf9185e5.el7 will be installed
    zfs: ---> Package perl-Carp.noarch 0:1.26-244.el7 will be installed
    zfs: ---> Package perl-Exporter.noarch 0:5.68-3.el7 will be installed
    zfs: ---> Package perl-File-Path.noarch 0:2.09-2.el7 will be installed
    zfs: ---> Package perl-File-Temp.noarch 0:0.23.01-3.el7 will be installed
    zfs: ---> Package perl-Filter.x86_64 0:1.49-3.el7 will be installed
    zfs: ---> Package perl-Getopt-Long.noarch 0:2.40-3.el7 will be installed
    zfs: --> Processing Dependency: perl(Pod::Usage) >= 1.14 for package: perl-Getopt-Long-2.40-3.el7.noarch
    zfs: --> Processing Dependency: perl(Text::ParseWords) for package: perl-Getopt-Long-2.40-3.el7.noarch
    zfs: ---> Package perl-PathTools.x86_64 0:3.40-5.el7 will be installed
    zfs: ---> Package perl-Pod-Simple.noarch 1:3.28-4.el7 will be installed
    zfs: --> Processing Dependency: perl(Pod::Escapes) >= 1.04 for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
    zfs: --> Processing Dependency: perl(Encode) for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
    zfs: ---> Package perl-Scalar-List-Utils.x86_64 0:1.27-248.el7 will be installed
    zfs: ---> Package perl-Socket.x86_64 0:2.010-5.el7 will be installed
    zfs: ---> Package perl-Storable.x86_64 0:2.45-3.el7 will be installed
    zfs: ---> Package perl-Time-HiRes.x86_64 4:1.9725-3.el7 will be installed
    zfs: ---> Package perl-Time-Local.noarch 0:1.2300-2.el7 will be installed
    zfs: ---> Package perl-constant.noarch 0:1.27-2.el7 will be installed
    zfs: ---> Package perl-libs.x86_64 4:5.16.3-299.el7_9 will be installed
    zfs: ---> Package perl-macros.x86_64 4:5.16.3-299.el7_9 will be installed
    zfs: ---> Package perl-threads.x86_64 0:1.87-4.el7 will be installed
    zfs: ---> Package perl-threads-shared.x86_64 0:1.43-6.el7 will be installed
    zfs: ---> Package zfs-dkms.noarch 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: dkms >= 2.2.0.3 for package: zfs-dkms-0.8.5-1.el7.noarch
    zfs: --> Running transaction check
    zfs: ---> Package cpp.x86_64 0:4.8.5-44.el7 will be installed
    zfs: ---> Package glibc-devel.x86_64 0:2.17-326.el7_9 will be installed
    zfs: --> Processing Dependency: glibc-headers = 2.17-326.el7_9 for package: glibc-devel-2.17-326.el7_9.x86_64
    zfs: --> Processing Dependency: glibc = 2.17-326.el7_9 for package: glibc-devel-2.17-326.el7_9.x86_64
    zfs: --> Processing Dependency: glibc-headers for package: glibc-devel-2.17-326.el7_9.x86_64
    zfs: ---> Package libgcc.x86_64 0:4.8.5-39.el7 will be updated
    zfs: ---> Package libgcc.x86_64 0:4.8.5-44.el7 will be an update
    zfs: ---> Package libgomp.x86_64 0:4.8.5-39.el7 will be updated
    zfs: ---> Package libgomp.x86_64 0:4.8.5-44.el7 will be an update
    zfs: ---> Package libmpc.x86_64 0:1.0.1-3.el7 will be installed
    zfs: ---> Package mpfr.x86_64 0:3.1.1-4.el7 will be installed
    zfs: ---> Package perl-Encode.x86_64 0:2.51-7.el7 will be installed
    zfs: ---> Package perl-Pod-Escapes.noarch 1:1.04-299.el7_9 will be installed
    zfs: ---> Package perl-Pod-Usage.noarch 0:1.63-3.el7 will be installed
    zfs: --> Processing Dependency: perl(Pod::Text) >= 3.15 for package: perl-Pod-Usage-1.63-3.el7.noarch
    zfs: --> Processing Dependency: perl-Pod-Perldoc for package: perl-Pod-Usage-1.63-3.el7.noarch
    zfs: ---> Package perl-Text-ParseWords.noarch 0:3.29-4.el7 will be installed
    zfs: ---> Package zfs-dkms.noarch 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: dkms >= 2.2.0.3 for package: zfs-dkms-0.8.5-1.el7.noarch
    zfs: --> Running transaction check
    zfs: ---> Package glibc.x86_64 0:2.17-307.el7.1 will be updated
    zfs: --> Processing Dependency: glibc = 2.17-307.el7.1 for package: glibc-common-2.17-307.el7.1.x86_64
    zfs: ---> Package glibc.x86_64 0:2.17-326.el7_9 will be an update
    zfs: ---> Package glibc-headers.x86_64 0:2.17-326.el7_9 will be installed
    zfs: --> Processing Dependency: kernel-headers >= 2.2.1 for package: glibc-headers-2.17-326.el7_9.x86_64
    zfs: --> Processing Dependency: kernel-headers for package: glibc-headers-2.17-326.el7_9.x86_64
    zfs: ---> Package perl-Pod-Perldoc.noarch 0:3.20-4.el7 will be installed
    zfs: --> Processing Dependency: perl(parent) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
    zfs: --> Processing Dependency: perl(HTTP::Tiny) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
    zfs: ---> Package perl-podlators.noarch 0:2.5.1-3.el7 will be installed
    zfs: ---> Package zfs-dkms.noarch 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: dkms >= 2.2.0.3 for package: zfs-dkms-0.8.5-1.el7.noarch
    zfs: --> Running transaction check
    zfs: ---> Package glibc-common.x86_64 0:2.17-307.el7.1 will be updated
    zfs: ---> Package glibc-common.x86_64 0:2.17-326.el7_9 will be an update
    zfs: ---> Package kernel-headers.x86_64 0:3.10.0-1160.90.1.el7 will be installed
    zfs: ---> Package perl-HTTP-Tiny.noarch 0:0.033-3.el7 will be installed
    zfs: ---> Package perl-parent.noarch 1:0.225-244.el7 will be installed
    zfs: ---> Package zfs-dkms.noarch 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: dkms >= 2.2.0.3 for package: zfs-dkms-0.8.5-1.el7.noarch
    zfs: --> Finished Dependency Resolution
    zfs:  You could try using --skip-broken to work around the problem
    zfs: Error: Package: zfs-dkms-0.8.5-1.el7.noarch (zfs)
    zfs:            Requires: dkms >= 2.2.0.3
    zfs:  You could try running: rpm -Va --nofiles --nodigest
    zfs: Loaded plugins: fastestmirror
    zfs: ================================== repo: zfs ===================================
    zfs: [zfs]
    zfs: async = True
    zfs: bandwidth = 0
    zfs: base_persistdir = /var/lib/yum/repos/x86_64/7
    zfs: baseurl = http://download.zfsonlinux.org/epel/7.8/x86_64/
    zfs: cache = 0
    zfs: cachedir = /var/cache/yum/x86_64/7/zfs
    zfs: check_config_file_age = True
    zfs: compare_providers_priority = 80
    zfs: cost = 1000
    zfs: deltarpm_metadata_percentage = 100
    zfs: deltarpm_percentage =
    zfs: enabled = 0
    zfs: enablegroups = True
    zfs: exclude =
    zfs: failovermethod = priority
    zfs: ftp_disable_epsv = False
    zfs: gpgcadir = /var/lib/yum/repos/x86_64/7/zfs/gpgcadir
    zfs: gpgcakey =
    zfs: gpgcheck = True
    zfs: gpgdir = /var/lib/yum/repos/x86_64/7/zfs/gpgdir
    zfs: gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-zfsonlinux
    zfs: hdrdir = /var/cache/yum/x86_64/7/zfs/headers
    zfs: http_caching = all
    zfs: includepkgs =
    zfs: ip_resolve =
    zfs: keepalive = True
    zfs: keepcache = False
    zfs: mddownloadpolicy = sqlite
    zfs: mdpolicy = group:small
    zfs: mediaid =
    zfs: metadata_expire = 604800
    zfs: metadata_expire_filter = read-only:present
    zfs: metalink =
    zfs: minrate = 0
    zfs: mirrorlist =
    zfs: mirrorlist_expire = 86400
    zfs: name = ZFS on Linux for EL7 - dkms
    zfs: old_base_cache_dir =
    zfs: password =
    zfs: persistdir = /var/lib/yum/repos/x86_64/7/zfs
    zfs: pkgdir = /var/cache/yum/x86_64/7/zfs/packages
    zfs: proxy = False
    zfs: proxy_dict =
    zfs: proxy_password =
    zfs: proxy_username =
    zfs: repo_gpgcheck = False
    zfs: retries = 10
    zfs: skip_if_unavailable = False
    zfs: ssl_check_cert_permissions = True
    zfs: sslcacert =
    zfs: sslclientcert =
    zfs: sslclientkey =
    zfs: sslverify = True
    zfs: throttle = 0
    zfs: timeout = 30.0
    zfs: ui_id = zfs/x86_64
    zfs: ui_repoid_vars = releasever,
    zfs:    basearch
    zfs: username =
    zfs: 
    zfs: Loaded plugins: fastestmirror
    zfs: ================================ repo: zfs-kmod ================================
    zfs: [zfs-kmod]
    zfs: async = True
    zfs: bandwidth = 0
    zfs: base_persistdir = /var/lib/yum/repos/x86_64/7
    zfs: baseurl = http://download.zfsonlinux.org/epel/7.8/kmod/x86_64/
    zfs: cache = 0
    zfs: cachedir = /var/cache/yum/x86_64/7/zfs-kmod
    zfs: check_config_file_age = True
    zfs: compare_providers_priority = 80
    zfs: cost = 1000
    zfs: deltarpm_metadata_percentage = 100
    zfs: deltarpm_percentage =
    zfs: enabled = 1
    zfs: enablegroups = True
    zfs: exclude =
    zfs: failovermethod = priority
    zfs: ftp_disable_epsv = False
    zfs: gpgcadir = /var/lib/yum/repos/x86_64/7/zfs-kmod/gpgcadir
    zfs: gpgcakey =
    zfs: gpgcheck = True
    zfs: gpgdir = /var/lib/yum/repos/x86_64/7/zfs-kmod/gpgdir
    zfs: gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-zfsonlinux
    zfs: hdrdir = /var/cache/yum/x86_64/7/zfs-kmod/headers
    zfs: http_caching = all
    zfs: includepkgs =
    zfs: ip_resolve =
    zfs: keepalive = True
    zfs: keepcache = False
    zfs: mddownloadpolicy = sqlite
    zfs: mdpolicy = group:small
    zfs: mediaid =
    zfs: metadata_expire = 604800
    zfs: metadata_expire_filter = read-only:present
    zfs: metalink =
    zfs: minrate = 0
    zfs: mirrorlist =
    zfs: mirrorlist_expire = 86400
    zfs: name = ZFS on Linux for EL7 - kmod
    zfs: old_base_cache_dir =
    zfs: password =
    zfs: persistdir = /var/lib/yum/repos/x86_64/7/zfs-kmod
    zfs: pkgdir = /var/cache/yum/x86_64/7/zfs-kmod/packages
    zfs: proxy = False
    zfs: proxy_dict =
    zfs: proxy_password =
    zfs: proxy_username =
    zfs: repo_gpgcheck = False
    zfs: retries = 10
    zfs: skip_if_unavailable = False
    zfs: ssl_check_cert_permissions = True
    zfs: sslcacert =
    zfs: sslclientcert =
    zfs: sslclientkey =
    zfs: sslverify = True
    zfs: throttle = 0
    zfs: timeout = 30.0
    zfs: ui_id = zfs-kmod/x86_64
    zfs: ui_repoid_vars = releasever,
    zfs:    basearch
    zfs: username =
    zfs: 
    zfs: Loaded plugins: fastestmirror
    zfs: Loading mirror speeds from cached hostfile
    zfs:  * base: mirror.23m.com
    zfs:  * extras: ftp.plusline.net
    zfs:  * updates: mirror.23m.com
    zfs: Resolving Dependencies
    zfs: --> Running transaction check
    zfs: ---> Package zfs.x86_64 0:0.8.5-1.el7 will be installed
    zfs: --> Processing Dependency: zfs-kmod = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzpool2 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzfs2 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libuutil1 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libnvpair1 = 0.8.5 for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: sysstat for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzpool.so.2()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzfs_core.so.1()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libzfs.so.2()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libuutil.so.1()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Processing Dependency: libnvpair.so.1()(64bit) for package: zfs-0.8.5-1.el7.x86_64
    zfs: --> Running transaction check
    zfs: ---> Package kmod-zfs.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libnvpair1.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libuutil1.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libzfs2.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package libzpool2.x86_64 0:0.8.5-1.el7 will be installed
    zfs: ---> Package sysstat.x86_64 0:10.1.5-20.el7_9 will be installed
    zfs: --> Processing Dependency: libsensors.so.4()(64bit) for package: sysstat-10.1.5-20.el7_9.x86_64
    zfs: --> Running transaction check
    zfs: ---> Package lm_sensors-libs.x86_64 0:3.4.0-8.20160601gitf9185e5.el7 will be installed
    zfs: --> Finished Dependency Resolution
    zfs: 
    zfs: Dependencies Resolved
    zfs: 
    zfs: ================================================================================
    zfs:  Package           Arch     Version                            Repository  Size
    zfs: ================================================================================
    zfs: Installing:
    zfs:  zfs               x86_64   0.8.5-1.el7                        zfs-kmod   486 k
    zfs: Installing for dependencies:
    zfs:  kmod-zfs          x86_64   0.8.5-1.el7                        zfs-kmod   1.1 M
    zfs:  libnvpair1        x86_64   0.8.5-1.el7                        zfs-kmod    32 k
    zfs:  libuutil1         x86_64   0.8.5-1.el7                        zfs-kmod    26 k
    zfs:  libzfs2           x86_64   0.8.5-1.el7                        zfs-kmod   208 k
    zfs:  libzpool2         x86_64   0.8.5-1.el7                        zfs-kmod   861 k
    zfs:  lm_sensors-libs   x86_64   3.4.0-8.20160601gitf9185e5.el7     base        42 k
    zfs:  sysstat           x86_64   10.1.5-20.el7_9                    updates    315 k
    zfs: 
    zfs: Transaction Summary
    zfs: ================================================================================
    zfs: Install  1 Package (+7 Dependent packages)
    zfs: 
    zfs: Total download size: 3.0 M
    zfs: Installed size: 11 M
    zfs: Downloading packages:
    zfs: Public key for lm_sensors-libs-3.4.0-8.20160601gitf9185e5.el7.x86_64.rpm is not installed
    zfs: warning: /var/cache/yum/x86_64/7/base/packages/lm_sensors-libs-3.4.0-8.20160601gitf9185e5.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID f4a80eb5: NOKEY
    zfs: Public key for sysstat-10.1.5-20.el7_9.x86_64.rpm is not installed
    zfs: --------------------------------------------------------------------------------
    zfs: Total                                              824 kB/s | 3.0 MB  00:03
    zfs: Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    zfs: Importing GPG key 0xF4A80EB5:
    zfs:  Userid     : "CentOS-7 Key (CentOS 7 Official Signing Key) <security@centos.org>"
    zfs:  Fingerprint: 6341 ab27 53d7 8a78 a7c2 7bb1 24c6 a8a7 f4a8 0eb5
    zfs:  Package    : centos-release-7-8.2003.0.el7.centos.x86_64 (@anaconda)
    zfs:  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    zfs: Running transaction check
    zfs: Running transaction test
    zfs: Transaction test succeeded
    zfs: Running transaction
    zfs:   Installing : libnvpair1-0.8.5-1.el7.x86_64                                1/8
    zfs:   Installing : libuutil1-0.8.5-1.el7.x86_64                                 2/8
    zfs:   Installing : libzfs2-0.8.5-1.el7.x86_64                                   3/8
    zfs:   Installing : libzpool2-0.8.5-1.el7.x86_64                                 4/8
    zfs:   Installing : lm_sensors-libs-3.4.0-8.20160601gitf9185e5.el7.x86_64        5/8
    zfs:   Installing : sysstat-10.1.5-20.el7_9.x86_64                               6/8
    zfs:   Installing : kmod-zfs-0.8.5-1.el7.x86_64                                  7/8
    zfs:   Installing : zfs-0.8.5-1.el7.x86_64                                       8/8
    zfs:   Verifying  : libuutil1-0.8.5-1.el7.x86_64                                 1/8
    zfs:   Verifying  : libzfs2-0.8.5-1.el7.x86_64                                   2/8
    zfs:   Verifying  : zfs-0.8.5-1.el7.x86_64                                       3/8
    zfs:   Verifying  : sysstat-10.1.5-20.el7_9.x86_64                               4/8
    zfs:   Verifying  : kmod-zfs-0.8.5-1.el7.x86_64                                  5/8
    zfs:   Verifying  : libnvpair1-0.8.5-1.el7.x86_64                                6/8
    zfs:   Verifying  : lm_sensors-libs-3.4.0-8.20160601gitf9185e5.el7.x86_64        7/8
    zfs:   Verifying  : libzpool2-0.8.5-1.el7.x86_64                                 8/8
    zfs: 
    zfs: Installed:
    zfs:   zfs.x86_64 0:0.8.5-1.el7
    zfs: 
    zfs: Dependency Installed:
    zfs:   kmod-zfs.x86_64 0:0.8.5-1.el7
    zfs:   libnvpair1.x86_64 0:0.8.5-1.el7
    zfs:   libuutil1.x86_64 0:0.8.5-1.el7
    zfs:   libzfs2.x86_64 0:0.8.5-1.el7
    zfs:   libzpool2.x86_64 0:0.8.5-1.el7
    zfs:   lm_sensors-libs.x86_64 0:3.4.0-8.20160601gitf9185e5.el7
    zfs:   sysstat.x86_64 0:10.1.5-20.el7_9
    zfs: 
    zfs: Complete!
    zfs: Loaded plugins: fastestmirror
    zfs: Loading mirror speeds from cached hostfile
    zfs:  * base: mirror.23m.com
    zfs:  * extras: ftp.plusline.net
    zfs:  * updates: mirror.23m.com
    zfs: Resolving Dependencies
    zfs: --> Running transaction check
    zfs: ---> Package wget.x86_64 0:1.14-18.el7_6.1 will be installed
    zfs: --> Finished Dependency Resolution
    zfs: 
    zfs: Dependencies Resolved
    zfs: 
    zfs: ================================================================================
    zfs:  Package        Arch             Version                   Repository      Size
    zfs: ================================================================================
    zfs: Installing:
    zfs:  wget           x86_64           1.14-18.el7_6.1           base           547 k
    zfs: 
    zfs: Transaction Summary
    zfs: ================================================================================
    zfs: Install  1 Package
    zfs: 
    zfs: Total download size: 547 k
    zfs: Installed size: 2.0 M
    zfs: Downloading packages:
    zfs: Running transaction check
    zfs: Running transaction test
    zfs: Transaction test succeeded
    zfs: Running transaction
    zfs:   Installing : wget-1.14-18.el7_6.1.x86_64                                  1/1
    zfs:   Verifying  : wget-1.14-18.el7_6.1.x86_64                                  1/1
    zfs: 
    zfs: Installed:
    zfs:   wget.x86_64 0:1.14-18.el7_6.1
    zfs: 
    zfs: Complete!
```
2. Заходим на сервер и дальнейшие команды выполняем от root

```
neva@Uneva:~$ vagrant ssh

[vagrant@zfs ~]$ sudo -i
```

3. Проверяем список дисков на ВМ:

```
[root@zfs ~]# lsblk
NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sda      8:0    0   40G  0 disk 
`-sda1   8:1    0   40G  0 part /
sdb      8:16   0  512M  0 disk 
sdc      8:32   0  512M  0 disk 
sdd      8:48   0  512M  0 disk 
sde      8:64   0  512M  0 disk 
sdf      8:80   0  512M  0 disk 
sdg      8:96   0  512M  0 disk 
sdh      8:112  0  512M  0 disk 
sdi      8:128  0  512M  0 disk 
```

4. Создадим 4 пула каждый из 2-х дисков в зеркале

```
zpool create otus1 mirror /dev/sdb /dev/sdc
zpool create otus2 mirror /dev/sdd /dev/sde
zpool create otus3 mirror /dev/sdf /dev/sdg
zpool create otus4 mirror /dev/sdh /dev/sdi
```

5. Проверяем созданные пулы:

```
[root@zfs ~]# zpool list
NAME    SIZE  ALLOC   FREE  CKPOINT  EXPANDSZ   FRAG    CAP  DEDUP    HEALTH  ALTROOT
otus1   480M  91.5K   480M        -         -     0%     0%  1.00x    ONLINE  -
otus2   480M  91.5K   480M        -         -     0%     0%  1.00x    ONLINE  -
otus3   480M  91.5K   480M        -         -     0%     0%  1.00x    ONLINE  -
otus4   480M  91.5K   480M        -         -     0%     0%  1.00x    ONLINE  -
[root@zfs ~]# zpool status
  pool: otus1
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus1       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdb     ONLINE       0     0     0
    sdc     ONLINE       0     0     0

errors: No known data errors

  pool: otus2
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus2       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdd     ONLINE       0     0     0
    sde     ONLINE       0     0     0

errors: No known data errors

  pool: otus3
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus3       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdf     ONLINE       0     0     0
    sdg     ONLINE       0     0     0

errors: No known data errors

  pool: otus4
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus4       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdh     ONLINE       0     0     0
    sdi     ONLINE       0     0     0

errors: No known data errors
```

6. Добавим разные алгоритмы сжатия в каждую файловую систему:

```
[root@zfs ~]# zfs set comrpression=lzjb otus1
[root@zfs ~]# zfs set compression=lz4 otus2
[root@zfs ~]# zfs set compression=gzip-9 otus3
[root@zfs ~]# zfs set compression=zle otus4
```

7. Проверим сжатие:

```
[root@zfs ~]# zfs get all | grep compression
otus1  compression           lzjb                   local
otus2  compression           lz4                    local
otus3  compression           gzip-9                 local
otus4  compression           zle                    local
```

8. Скачаем один и тот же текстовый файл во все пулы: 

```
[root@zfs ~]# for i in {1..4}; do wget -P /otus$i https://gutenberg.org/cache/epub/2600/pg2600.converter.log; done
--2023-05-23 07:04:25--  https://gutenberg.org/cache/epub/2600/pg2600.converter.log
Resolving gutenberg.org (gutenberg.org)... 152.19.134.47, 2610:28:3090:3000:0:bad:cafe:47
Connecting to gutenberg.org (gutenberg.org)|152.19.134.47|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 40931771 (39M) [text/plain]
Saving to: '/otus1/pg2600.converter.log'


 0% [                                                                                                                                                                                                    ] 0           --.-K/s              
 0% [                                                                                                                                                                                                    ] 44,057       152KB/s             
 0% [>                                                                                                                                                                                                   ] 214,061      367KB/s             
 0% [>                                                                                                                                                                                                   ] 394,285      448KB/s             
 2% [===>                                                                                                                                                                                                ] 1,000,493    769KB/s             
 3% [=====>                                                                                                                                                                                              ] 1,442,861    954KB/s             
 4% [=======>                                                                                                                                                                                            ] 1,688,621    968KB/s             
 4% [========>                                                                                                                                                                                           ] 1,917,997    984KB/s             
 5% [=========>                                                                                                                                                                                          ] 2,180,141   1003KB/s             
 5% [==========>                                                                                                                                                                                         ] 2,425,901   1019KB/s             
 6% [============>                                                                                                                                                                                       ] 2,720,813   1.02MB/s             
 7% [=============>                                                                                                                                                                                      ] 2,999,341   1.04MB/s             
 8% [==============>                                                                                                                                                                                     ] 3,294,253   1.06MB/s             
 8% [================>                                                                                                                                                                                   ] 3,572,781   1.07MB/s  eta 33s    
 9% [=================>                                                                                                                                                                                  ] 3,884,077   1.09MB/s  eta 33s    
10% [===================>                                                                                                                                                                                ] 4,178,989   1.10MB/s  eta 33s    
10% [====================>                                                                                                                                                                               ] 4,490,285   1.12MB/s  eta 33s    
11% [=====================>                                                                                                                                                                              ] 4,785,197   1.13MB/s  eta 33s    
12% [=======================>                                                                                                                                                                            ] 5,112,877   1.23MB/s  eta 30s    
13% [========================>                                                                                                                                                                           ] 5,407,789   1.33MB/s  eta 30s    
13% [==========================>                                                                                                                                                                         ] 5,719,085   1.33MB/s  eta 30s    
14% [===========================>                                                                                                                                                                        ] 6,030,381   1.29MB/s  eta 30s    
15% [=============================>                                                                                                                                                                      ] 6,341,677   1.32MB/s  eta 30s    
16% [==============================>                                                                                                                                                                     ] 6,636,589   1.34MB/s  eta 27s    
16% [================================>                                                                                                                                                                   ] 6,931,501   1.35MB/s  eta 27s    
17% [=================================>                                                                                                                                                                  ] 7,275,565   1.38MB/s  eta 27s    
18% [===================================>                                                                                                                                                                ] 7,586,861   1.38MB/s  eta 27s    
19% [====================================>                                                                                                                                                               ] 7,930,925   1.40MB/s  eta 27s    
20% [======================================>                                                                                                                                                             ] 8,225,837   1.40MB/s  eta 25s    
20% [========================================>                                                                                                                                                           ] 8,569,901   1.41MB/s  eta 25s    
21% [=========================================>                                                                                                                                                          ] 8,864,813   1.41MB/s  eta 25s    
22% [==========================================>                                                                                                                                                         ] 9,159,725   1.42MB/s  eta 25s    
23% [============================================>                                                                                                                                                       ] 9,503,789   1.42MB/s  eta 25s    
24% [==============================================>                                                                                                                                                     ] 9,831,469   1.43MB/s  eta 23s    
24% [===============================================>                                                                                                                                                    ] 10,159,149  1.42MB/s  eta 23s    
25% [=================================================>                                                                                                                                                  ] 10,454,061  1.42MB/s  eta 23s    
26% [==================================================>                                                                                                                                                 ] 10,798,125  1.42MB/s  eta 23s    
27% [====================================================>                                                                                                                                               ] 11,093,037  1.42MB/s  eta 23s    
27% [=====================================================>                                                                                                                                              ] 11,453,485  1.43MB/s  eta 22s    
28% [=======================================================>                                                                                                                                            ] 11,764,781  1.44MB/s  eta 22s    
29% [=========================================================>                                                                                                                                          ] 12,125,229  1.44MB/s  eta 22s    
30% [==========================================================>                                                                                                                                         ] 12,469,293  1.44MB/s  eta 22s    
31% [============================================================>                                                                                                                                       ] 12,813,357  1.44MB/s  eta 22s    
32% [==============================================================>                                                                                                                                     ] 13,173,805  1.47MB/s  eta 20s    
33% [===============================================================>                                                                                                                                    ] 13,517,869  1.47MB/s  eta 20s    
33% [=================================================================>                                                                                                                                  ] 13,861,933  1.48MB/s  eta 20s    
34% [===================================================================>                                                                                                                                ] 14,238,765  1.50MB/s  eta 20s    
35% [====================================================================>                                                                                                                               ] 14,599,213  1.50MB/s  eta 20s    
36% [======================================================================>                                                                                                                             ] 15,008,813  1.52MB/s  eta 18s    
37% [========================================================================>                                                                                                                           ] 15,385,645  1.54MB/s  eta 18s    
38% [==========================================================================>                                                                                                                         ] 15,811,629  1.57MB/s  eta 18s    
39% [============================================================================>                                                                                                                       ] 16,221,229  1.61MB/s  eta 18s    
40% [==============================================================================>                                                                                                                     ] 16,663,597  1.63MB/s  eta 18s    
41% [================================================================================>                                                                                                                   ] 17,105,965  1.66MB/s  eta 16s    
42% [===================================================================================>                                                                                                                ] 17,581,101  1.70MB/s  eta 16s    
44% [=====================================================================================>                                                                                                              ] 18,056,237  1.74MB/s  eta 16s    
45% [=======================================================================================>                                                                                                            ] 18,564,141  1.80MB/s  eta 16s    
46% [==========================================================================================>                                                                                                         ] 19,072,045  1.85MB/s  eta 16s    
47% [============================================================================================>                                                                                                       ] 19,629,101  1.91MB/s  eta 14s    
49% [===============================================================================================>                                                                                                    ] 20,186,157  1.96MB/s  eta 14s    
50% [==================================================================================================>                                                                                                 ] 20,792,365  2.03MB/s  eta 14s    
52% [=====================================================================================================>                                                                                              ] 21,398,573  2.11MB/s  eta 14s    
53% [========================================================================================================>                                                                                           ] 22,053,933  2.21MB/s  eta 14s    
55% [===========================================================================================================>                                                                                        ] 22,725,677  2.28MB/s  eta 11s    
57% [===============================================================================================================>                                                                                    ] 23,446,573  2.36MB/s  eta 11s    
59% [==================================================================================================================>                                                                                 ] 24,183,853  2.49MB/s  eta 11s    
60% [=====================================================================================================================>                                                                              ] 24,806,445  2.45MB/s  eta 11s    
63% [===========================================================================================================================>                                                                        ] 26,002,477  2.68MB/s  eta 9s     
64% [==============================================================================================================================>                                                                     ] 26,592,301  2.70MB/s  eta 9s     
66% [=================================================================================================================================>                                                                  ] 27,198,509  2.74MB/s  eta 9s     
67% [====================================================================================================================================>                                                               ] 27,821,101  2.78MB/s  eta 9s     
69% [=======================================================================================================================================>                                                            ] 28,410,925  2.83MB/s  eta 9s     
70% [==========================================================================================================================================>                                                         ] 29,049,901  2.87MB/s  eta 6s     
72% [=============================================================================================================================================>                                                      ] 29,672,493  2.91MB/s  eta 6s     
74% [================================================================================================================================================>                                                   ] 30,311,469  2.92MB/s  eta 6s     
75% [==================================================================================================================================================>                                                 ] 30,819,373  2.78MB/s  eta 6s     
77% [======================================================================================================================================================>                                             ] 31,638,573  2.77MB/s  eta 5s     
79% [==========================================================================================================================================================>                                         ] 32,457,773  2.71MB/s  eta 5s     
81% [==============================================================================================================================================================>                                     ] 33,227,821  2.76MB/s  eta 5s     
82% [================================================================================================================================================================>                                   ] 33,653,805  2.71MB/s  eta 5s     
82% [=================================================================================================================================================================>                                  ] 33,965,101  2.61MB/s  eta 5s     
84% [===================================================================================================================================================================>                                ] 34,391,085  2.56MB/s  eta 3s     
84% [=====================================================================================================================================================================>                              ] 34,751,533  2.58MB/s  eta 3s     
85% [=======================================================================================================================================================================>                            ] 35,177,517  2.38MB/s  eta 3s     
86% [=========================================================================================================================================================================>                          ] 35,554,349  2.34MB/s  eta 3s     
87% [===========================================================================================================================================================================>                        ] 35,963,949  2.28MB/s  eta 3s     
88% [=============================================================================================================================================================================>                      ] 36,389,933  2.23MB/s  eta 2s     
89% [===============================================================================================================================================================================>                    ] 36,799,533  2.20MB/s  eta 2s     
90% [=================================================================================================================================================================================>                  ] 37,241,901  2.10MB/s  eta 2s     
92% [===================================================================================================================================================================================>                ] 37,667,885  2.06MB/s  eta 2s     
93% [=====================================================================================================================================================================================>              ] 38,110,253  2.01MB/s  eta 2s     
94% [=======================================================================================================================================================================================>            ] 38,503,469  2.04MB/s  eta 1s     
95% [=========================================================================================================================================================================================>          ] 38,994,989  1.98MB/s  eta 1s     
96% [===========================================================================================================================================================================================>        ] 39,404,589  1.85MB/s  eta 1s     
97% [=============================================================================================================================================================================================>      ] 39,863,341  1.87MB/s  eta 1s     
98% [===============================================================================================================================================================================================>    ] 40,272,941  1.87MB/s  eta 1s     
99% [==================================================================================================================================================================================================> ] 40,748,077  1.88MB/s  eta 0s     
100%[===================================================================================================================================================================================================>] 40,931,771  1.91MB/s   in 21s    

2023-05-23 07:04:47 (1.83 MB/s) - '/otus1/pg2600.converter.log' saved [40931771/40931771]

--2023-05-23 07:04:47--  https://gutenberg.org/cache/epub/2600/pg2600.converter.log
Resolving gutenberg.org (gutenberg.org)... 152.19.134.47, 2610:28:3090:3000:0:bad:cafe:47
Connecting to gutenberg.org (gutenberg.org)|152.19.134.47|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 40931771 (39M) [text/plain]
Saving to: '/otus2/pg2600.converter.log'


 0% [                                                                                                                                                                                                    ] 0           --.-K/s              
 0% [                                                                                                                                                                                                    ] 102,905      356KB/s             
 0% [>                                                                                                                                                                                                   ] 332,281      507KB/s             
 1% [==>                                                                                                                                                                                                 ] 709,113      812KB/s             
 2% [===>                                                                                                                                                                                                ] 987,641      914KB/s             
 2% [====>                                                                                                                                                                                               ] 1,184,249    921KB/s             
 3% [======>                                                                                                                                                                                             ] 1,561,081   1.01MB/s             
 4% [=======>                                                                                                                                                                                            ] 1,774,073   1.01MB/s             
 5% [=========>                                                                                                                                                                                          ] 2,167,289   1.10MB/s             
 5% [==========>                                                                                                                                                                                         ] 2,413,049   1.10MB/s             
 6% [============>                                                                                                                                                                                       ] 2,822,649   1.15MB/s             
 7% [==============>                                                                                                                                                                                     ] 3,183,097   1.19MB/s             
 8% [===============>                                                                                                                                                                                    ] 3,494,393   1.21MB/s             
 9% [=================>                                                                                                                                                                                  ] 3,854,841   1.24MB/s             
10% [===================>                                                                                                                                                                                ] 4,198,905   1.25MB/s  eta 28s    
11% [====================>                                                                                                                                                                               ] 4,592,121   1.29MB/s  eta 28s    
11% [======================>                                                                                                                                                                             ] 4,903,417   1.30MB/s  eta 28s    
12% [========================>                                                                                                                                                                           ] 5,280,249   1.32MB/s  eta 28s    
13% [=========================>                                                                                                                                                                          ] 5,624,313   1.50MB/s  eta 28s    
14% [===========================>                                                                                                                                                                        ] 6,001,145   1.51MB/s  eta 25s    
15% [=============================>                                                                                                                                                                      ] 6,361,593   1.52MB/s  eta 25s    
16% [===============================>                                                                                                                                                                    ] 6,738,425   1.54MB/s  eta 25s    
17% [================================>                                                                                                                                                                   ] 7,098,873   1.58MB/s  eta 25s    
18% [==================================>                                                                                                                                                                 ] 7,475,705   1.57MB/s  eta 25s    
19% [====================================>                                                                                                                                                               ] 7,852,537   1.58MB/s  eta 22s    
20% [======================================>                                                                                                                                                             ] 8,311,289   1.64MB/s  eta 22s    
20% [========================================>                                                                                                                                                           ] 8,589,817   1.63MB/s  eta 22s    
22% [==========================================>                                                                                                                                                         ] 9,032,185   1.65MB/s  eta 22s    
22% [===========================================>                                                                                                                                                        ] 9,327,097   1.63MB/s  eta 22s    
23% [=============================================>                                                                                                                                                      ] 9,785,849   1.65MB/s  eta 20s    
24% [===============================================>                                                                                                                                                    ] 10,113,529  1.66MB/s  eta 20s    
25% [=================================================>                                                                                                                                                  ] 10,523,129  1.66MB/s  eta 20s    
26% [===================================================>                                                                                                                                                ] 10,899,961  1.67MB/s  eta 20s    
27% [====================================================>                                                                                                                                               ] 11,260,409  1.66MB/s  eta 20s    
28% [======================================================>                                                                                                                                             ] 11,637,241  1.68MB/s  eta 19s    
29% [========================================================>                                                                                                                                           ] 12,014,073  1.69MB/s  eta 19s    
30% [==========================================================>                                                                                                                                         ] 12,366,329  1.68MB/s  eta 19s    
31% [============================================================>                                                                                                                                       ] 12,751,353  1.67MB/s  eta 19s    
31% [=============================================================>                                                                                                                                      ] 13,095,417  1.69MB/s  eta 19s    
33% [===============================================================>                                                                                                                                    ] 13,521,401  1.71MB/s  eta 17s    
33% [=================================================================>                                                                                                                                  ] 13,849,081  1.70MB/s  eta 17s    
34% [===================================================================>                                                                                                                                ] 14,291,449  1.70MB/s  eta 17s    
35% [=====================================================================>                                                                                                                              ] 14,635,513  1.70MB/s  eta 17s    
36% [=======================================================================>                                                                                                                            ] 15,094,265  1.72MB/s  eta 17s    
37% [========================================================================>                                                                                                                           ] 15,438,329  1.74MB/s  eta 16s    
38% [===========================================================================>                                                                                                                        ] 15,897,081  1.76MB/s  eta 16s    
39% [============================================================================>                                                                                                                       ] 16,273,913  1.74MB/s  eta 16s    
40% [===============================================================================>                                                                                                                    ] 16,749,049  1.79MB/s  eta 16s    
41% [=================================================================================>                                                                                                                  ] 17,125,881  1.80MB/s  eta 16s    
43% [===================================================================================>                                                                                                                ] 17,650,169  1.83MB/s  eta 14s    
44% [=====================================================================================>                                                                                                              ] 18,027,001  1.82MB/s  eta 14s    
45% [=======================================================================================>                                                                                                            ] 18,584,057  1.88MB/s  eta 14s    
46% [=========================================================================================>                                                                                                          ] 18,960,889  1.89MB/s  eta 14s    
47% [============================================================================================>                                                                                                       ] 19,550,713  1.95MB/s  eta 14s    
48% [==============================================================================================>                                                                                                     ] 19,993,081  1.99MB/s  eta 12s    
50% [=================================================================================================>                                                                                                  ] 20,533,753  2.03MB/s  eta 12s    
51% [===================================================================================================>                                                                                                ] 21,058,041  2.06MB/s  eta 12s    
52% [======================================================================================================>                                                                                             ] 21,631,481  2.11MB/s  eta 12s    
54% [=========================================================================================================>                                                                                          ] 22,237,689  2.18MB/s  eta 12s    
55% [============================================================================================================>                                                                                       ] 22,860,281  2.26MB/s  eta 10s    
57% [===============================================================================================================>                                                                                    ] 23,515,641  2.32MB/s  eta 10s    
58% [=================================================================================================================>                                                                                  ] 23,876,089  2.24MB/s  eta 10s    
60% [======================================================================================================================>                                                                             ] 24,859,129  2.40MB/s  eta 10s    
61% [========================================================================================================================>                                                                           ] 25,350,649  2.42MB/s  eta 10s    
63% [==========================================================================================================================>                                                                         ] 25,858,553  2.47MB/s  eta 8s     
64% [=============================================================================================================================>                                                                      ] 26,399,225  2.48MB/s  eta 8s     
65% [===============================================================================================================================>                                                                    ] 26,923,513  2.49MB/s  eta 8s     
67% [==================================================================================================================================>                                                                 ] 27,513,337  2.51MB/s  eta 8s     
68% [=====================================================================================================================================>                                                              ] 28,021,241  2.51MB/s  eta 8s     
70% [========================================================================================================================================>                                                           ] 28,676,601  2.56MB/s  eta 6s     
71% [==========================================================================================================================================>                                                         ] 29,217,273  2.58MB/s  eta 6s     
73% [==============================================================================================================================================>                                                     ] 29,905,401  2.61MB/s  eta 6s     
73% [===============================================================================================================================================>                                                    ] 30,200,313  2.48MB/s  eta 6s     
75% [===================================================================================================================================================>                                                ] 31,052,281  2.54MB/s  eta 6s     
77% [======================================================================================================================================================>                                             ] 31,560,185  2.51MB/s  eta 5s     
78% [========================================================================================================================================================>                                           ] 31,953,401  2.45MB/s  eta 5s     
79% [==========================================================================================================================================================>                                         ] 32,494,073  2.44MB/s  eta 5s     
80% [============================================================================================================================================================>                                       ] 32,903,673  2.50MB/s  eta 5s     
81% [===============================================================================================================================================================>                                    ] 33,493,497  2.39MB/s  eta 5s     
82% [=================================================================================================================================================================>                                  ] 33,935,865  2.37MB/s  eta 4s     
84% [====================================================================================================================================================================>                               ] 34,476,537  2.38MB/s  eta 4s     
85% [======================================================================================================================================================================>                             ] 34,902,521  2.36MB/s  eta 4s     
86% [========================================================================================================================================================================>                           ] 35,492,345  2.35MB/s  eta 4s     
87% [===========================================================================================================================================================================>                        ] 35,934,713  2.32MB/s  eta 4s     
89% [=============================================================================================================================================================================>                      ] 36,540,921  2.33MB/s  eta 2s     
90% [================================================================================================================================================================================>                   ] 36,983,289  2.29MB/s  eta 2s     
91% [==================================================================================================================================================================================>                 ] 37,589,497  2.31MB/s  eta 2s     
92% [=====================================================================================================================================================================================>              ] 38,031,865  2.34MB/s  eta 2s     
94% [========================================================================================================================================================================================>           ] 38,654,457  2.27MB/s  eta 2s     
95% [==========================================================================================================================================================================================>         ] 39,096,825  2.29MB/s  eta 1s     
97% [=============================================================================================================================================================================================>      ] 39,719,417  2.34MB/s  eta 1s     
98% [===============================================================================================================================================================================================>    ] 40,161,785  2.33MB/s  eta 1s     
99% [==================================================================================================================================================================================================> ] 40,784,377  2.36MB/s  eta 1s     
100%[===================================================================================================================================================================================================>] 40,931,771  2.35MB/s   in 20s    

2023-05-23 07:05:08 (1.97 MB/s) - '/otus2/pg2600.converter.log' saved [40931771/40931771]

--2023-05-23 07:05:08--  https://gutenberg.org/cache/epub/2600/pg2600.converter.log
Resolving gutenberg.org (gutenberg.org)... 152.19.134.47, 2610:28:3090:3000:0:bad:cafe:47
Connecting to gutenberg.org (gutenberg.org)|152.19.134.47|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 40931771 (39M) [text/plain]
Saving to: '/otus3/pg2600.converter.log'


 0% [                                                                                                                                                                                                    ] 0           --.-K/s              
 0% [                                                                                                                                                                                                    ] 44,057       152KB/s             
 0% [>                                                                                                                                                                                                   ] 218,945      376KB/s             
 1% [=>                                                                                                                                                                                                  ] 563,009      631KB/s             
 2% [===>                                                                                                                                                                                                ] 1,005,377    863KB/s             
 3% [=====>                                                                                                                                                                                              ] 1,447,745    991KB/s             
 4% [======>                                                                                                                                                                                             ] 1,660,737    900KB/s             
 5% [==========>                                                                                                                                                                                         ] 2,365,249   1.12MB/s             
 6% [============>                                                                                                                                                                                       ] 2,807,617   1.17MB/s             
 7% [=============>                                                                                                                                                                                      ] 3,020,609   1.14MB/s             
 8% [================>                                                                                                                                                                                   ] 3,610,433   1.26MB/s             
 9% [=================>                                                                                                                                                                                  ] 3,905,345   1.25MB/s             
10% [===================>                                                                                                                                                                                ] 4,331,329   1.26MB/s  eta 28s    
11% [=====================>                                                                                                                                                                              ] 4,773,697   1.28MB/s  eta 28s    
12% [========================>                                                                                                                                                                           ] 5,232,449   1.30MB/s  eta 28s    
13% [==========================>                                                                                                                                                                         ] 5,707,585   1.41MB/s  eta 28s    
15% [============================>                                                                                                                                                                       ] 6,166,337   1.48MB/s  eta 24s    
15% [=============================>                                                                                                                                                                      ] 6,444,865   1.54MB/s  eta 24s    
16% [===============================>                                                                                                                                                                    ] 6,838,081   1.55MB/s  eta 24s    
17% [=================================>                                                                                                                                                                  ] 7,214,913   1.53MB/s  eta 24s    
18% [===================================>                                                                                                                                                                ] 7,690,049   1.56MB/s  eta 24s    
19% [=====================================>                                                                                                                                                              ] 8,001,345   1.69MB/s  eta 22s    
20% [=======================================>                                                                                                                                                            ] 8,460,097   1.63MB/s  eta 22s    
21% [=========================================>                                                                                                                                                          ] 8,787,777   1.60MB/s  eta 22s    
22% [==========================================>                                                                                                                                                         ] 9,180,993   1.69MB/s  eta 22s    
23% [============================================>                                                                                                                                                       ] 9,590,593   1.65MB/s  eta 22s    
24% [==============================================>                                                                                                                                                     ] 9,918,273   1.66MB/s  eta 20s    
25% [================================================>                                                                                                                                                   ] 10,409,793  1.67MB/s  eta 20s    
26% [==================================================>                                                                                                                                                 ] 10,835,777  1.70MB/s  eta 20s    
27% [====================================================>                                                                                                                                               ] 11,228,993  1.74MB/s  eta 20s    
28% [=======================================================>                                                                                                                                            ] 11,769,665  1.76MB/s  eta 20s    
30% [=========================================================>                                                                                                                                          ] 12,310,337  1.74MB/s  eta 18s    
31% [============================================================>                                                                                                                                       ] 12,851,009  1.78MB/s  eta 18s    
32% [==============================================================>                                                                                                                                     ] 13,162,305  1.58MB/s  eta 18s    
32% [==============================================================>                                                                                                                                     ] 13,252,417  1.39MB/s  eta 19s    
36% [======================================================================>                                                                                                                             ] 14,849,857  1.63MB/s  eta 19s    
37% [=======================================================================>                                                                                                                            ] 15,210,305  1.65MB/s  eta 19s    
37% [=========================================================================>                                                                                                                          ] 15,521,601  1.63MB/s  eta 19s    
38% [===========================================================================>                                                                                                                        ] 15,882,049  1.60MB/s  eta 19s    
39% [============================================================================>                                                                                                                       ] 16,226,113  1.59MB/s  eta 16s    
40% [==============================================================================>                                                                                                                     ] 16,668,481  1.61MB/s  eta 16s    
41% [================================================================================>                                                                                                                   ] 16,963,393  1.59MB/s  eta 16s    
42% [==================================================================================>                                                                                                                 ] 17,405,761  1.58MB/s  eta 16s    
43% [===================================================================================>                                                                                                                ] 17,733,441  1.56MB/s  eta 16s    
44% [======================================================================================>                                                                                                             ] 18,175,809  1.58MB/s  eta 14s    
45% [=======================================================================================>                                                                                                            ] 18,503,489  1.58MB/s  eta 14s    
46% [=========================================================================================>                                                                                                          ] 18,962,241  1.58MB/s  eta 14s    
47% [===========================================================================================>                                                                                                        ] 19,289,921  1.56MB/s  eta 14s    
48% [=============================================================================================>                                                                                                      ] 19,699,521  1.55MB/s  eta 14s    
49% [===============================================================================================>                                                                                                    ] 20,092,737  1.76MB/s  eta 13s    
50% [=================================================================================================>                                                                                                  ] 20,502,337  2.03MB/s  eta 13s    
51% [===================================================================================================>                                                                                                ] 20,911,937  1.68MB/s  eta 13s    
51% [====================================================================================================>                                                                                               ] 21,174,081  1.65MB/s  eta 13s    
51% [====================================================================================================>                                                                                               ] 21,239,617  1.50MB/s  eta 12s    
52% [=====================================================================================================>                                                                                              ] 21,354,305  1.42MB/s  eta 12s    
53% [=======================================================================================================>                                                                                            ] 21,780,289  1.39MB/s  eta 12s    
57% [==============================================================================================================>                                                                                     ] 23,369,537  1.71MB/s  eta 12s    
57% [================================================================================================================>                                                                                   ] 23,680,833  1.68MB/s  eta 11s    
59% [==================================================================================================================>                                                                                 ] 24,172,353  1.71MB/s  eta 11s    
59% [====================================================================================================================>                                                                               ] 24,500,033  1.70MB/s  eta 11s    
61% [======================================================================================================================>                                                                             ] 24,991,553  1.72MB/s  eta 11s    
61% [========================================================================================================================>                                                                           ] 25,319,233  1.72MB/s  eta 11s    
63% [==========================================================================================================================>                                                                         ] 25,810,753  1.73MB/s  eta 9s     
63% [============================================================================================================================>                                                                       ] 26,138,433  1.72MB/s  eta 9s     
65% [==============================================================================================================================>                                                                     ] 26,629,953  1.73MB/s  eta 9s     
65% [================================================================================================================================>                                                                   ] 26,957,633  1.72MB/s  eta 9s     
67% [==================================================================================================================================>                                                                 ] 27,465,537  1.75MB/s  eta 9s     
67% [====================================================================================================================================>                                                               ] 27,793,217  1.73MB/s  eta 8s     
69% [======================================================================================================================================>                                                             ] 28,317,505  1.76MB/s  eta 8s     
69% [========================================================================================================================================>                                                           ] 28,645,185  1.80MB/s  eta 8s     
71% [==========================================================================================================================================>                                                         ] 29,185,857  2.12MB/s  eta 8s     
72% [============================================================================================================================================>                                                       ] 29,513,537  2.15MB/s  eta 8s     
73% [===============================================================================================================================================>                                                    ] 30,086,977  1.87MB/s  eta 6s     
74% [================================================================================================================================================>                                                   ] 30,463,809  1.86MB/s  eta 6s     
74% [=================================================================================================================================================>                                                  ] 30,693,185  1.62MB/s  eta 6s     
75% [==================================================================================================================================================>                                                 ] 30,709,569  1.42MB/s  eta 6s     
79% [=========================================================================================================================================================>                                          ] 32,364,353  1.71MB/s  eta 6s     
79% [===========================================================================================================================================================>                                        ] 32,659,265  1.68MB/s  eta 6s     
80% [============================================================================================================================================================>                                       ] 32,872,257  1.64MB/s  eta 6s     
81% [=============================================================================================================================================================>                                      ] 33,199,937  1.63MB/s  eta 6s     
81% [==============================================================================================================================================================>                                     ] 33,412,929  1.58MB/s  eta 5s     
82% [================================================================================================================================================================>                                   ] 33,756,993  1.56MB/s  eta 5s     
83% [=================================================================================================================================================================>                                  ] 34,035,521  1.52MB/s  eta 5s     
83% [===================================================================================================================================================================>                                ] 34,330,433  1.50MB/s  eta 5s     
84% [====================================================================================================================================================================>                               ] 34,641,729  1.48MB/s  eta 5s     
85% [======================================================================================================================================================================>                             ] 34,920,257  1.45MB/s  eta 4s     
85% [=======================================================================================================================================================================>                            ] 35,149,633  1.42MB/s  eta 4s     
86% [=========================================================================================================================================================================>                          ] 35,510,081  1.39MB/s  eta 4s     
87% [==========================================================================================================================================================================>                         ] 35,739,457  1.35MB/s  eta 4s     
88% [===========================================================================================================================================================================>                        ] 36,099,905  1.34MB/s  eta 4s     
88% [=============================================================================================================================================================================>                      ] 36,345,665  1.30MB/s  eta 3s     
89% [==============================================================================================================================================================================>                     ] 36,706,113  1.47MB/s  eta 3s     
90% [===============================================================================================================================================================================>                    ] 36,935,489  1.64MB/s  eta 3s     
91% [=================================================================================================================================================================================>                  ] 37,295,937  1.28MB/s  eta 3s     
91% [==================================================================================================================================================================================>                 ] 37,492,545  1.23MB/s  eta 3s     
92% [====================================================================================================================================================================================>               ] 37,918,529  1.29MB/s  eta 2s     
93% [=====================================================================================================================================================================================>              ] 38,197,057  1.26MB/s  eta 2s     
93% [======================================================================================================================================================================================>             ] 38,377,281  1.24MB/s  eta 2s     
94% [========================================================================================================================================================================================>           ] 38,655,809  1.23MB/s  eta 2s     
95% [=========================================================================================================================================================================================>          ] 38,983,489  1.24MB/s  eta 2s     
95% [==========================================================================================================================================================================================>         ] 39,180,097  1.20MB/s  eta 1s     
96% [============================================================================================================================================================================================>       ] 39,507,777  1.19MB/s  eta 1s     
97% [=============================================================================================================================================================================================>      ] 39,802,689  1.21MB/s  eta 1s     
97% [==============================================================================================================================================================================================>     ] 40,048,449  1.17MB/s  eta 1s     
98% [================================================================================================================================================================================================>   ] 40,359,745  1.18MB/s  eta 1s     
99% [=================================================================================================================================================================================================>  ] 40,605,505  1.17MB/s  eta 0s     
100%[===================================================================================================================================================================================================>] 40,931,771  1.19MB/s   in 26s    

2023-05-23 07:05:34 (1.51 MB/s) - '/otus3/pg2600.converter.log' saved [40931771/40931771]

--2023-05-23 07:05:34--  https://gutenberg.org/cache/epub/2600/pg2600.converter.log
Resolving gutenberg.org (gutenberg.org)... 152.19.134.47, 2610:28:3090:3000:0:bad:cafe:47
Connecting to gutenberg.org (gutenberg.org)|152.19.134.47|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 40931771 (39M) [text/plain]
Saving to: '/otus4/pg2600.converter.log'


 0% [                                                                                                                                                                                                    ] 0           --.-K/s              
 0% [                                                                                                                                                                                                    ] 40,051       142KB/s             
 0% [>                                                                                                                                                                                                   ] 220,275      391KB/s             
 1% [=>                                                                                                                                                                                                  ] 515,187      608KB/s             
 1% [==>                                                                                                                                                                                                 ] 810,099      716KB/s             
 2% [====>                                                                                                                                                                                               ] 1,121,395    791KB/s             
 3% [=====>                                                                                                                                                                                              ] 1,318,003    811KB/s             
 3% [======>                                                                                                                                                                                             ] 1,580,147    806KB/s             
 4% [========>                                                                                                                                                                                           ] 1,891,443    870KB/s             
 5% [========>                                                                                                                                                                                           ] 2,071,667    866KB/s             
 5% [=========>                                                                                                                                                                                          ] 2,235,507    857KB/s             
 5% [==========>                                                                                                                                                                                         ] 2,448,499    862KB/s             
 6% [===========>                                                                                                                                                                                        ] 2,694,259    870KB/s  eta 43s    
 7% [============>                                                                                                                                                                                       ] 2,890,867    870KB/s  eta 43s    
 7% [==============>                                                                                                                                                                                     ] 3,136,627    882KB/s  eta 43s    
 8% [===============>                                                                                                                                                                                    ] 3,398,771    893KB/s  eta 43s    
 8% [================>                                                                                                                                                                                   ] 3,595,379    897KB/s  eta 43s    
 9% [=================>                                                                                                                                                                                  ] 3,857,523    967KB/s  eta 40s    
 9% [==================>                                                                                                                                                                                 ] 4,070,515    983KB/s  eta 40s    
10% [===================>                                                                                                                                                                                ] 4,332,659    975KB/s  eta 40s    
11% [====================>                                                                                                                                                                               ] 4,545,651    992KB/s  eta 40s    
11% [======================>                                                                                                                                                                             ] 4,807,795    979KB/s  eta 40s    
12% [======================>                                                                                                                                                                             ] 5,004,403   1002KB/s  eta 37s    
12% [========================>                                                                                                                                                                           ] 5,282,931   1.01MB/s  eta 37s    
13% [=========================>                                                                                                                                                                          ] 5,479,539    996KB/s  eta 37s    
14% [==========================>                                                                                                                                                                         ] 5,758,067   1.00MB/s  eta 37s    
14% [===========================>                                                                                                                                                                        ] 5,954,675   1.01MB/s  eta 37s    
15% [============================>                                                                                                                                                                       ] 6,233,203   1.04MB/s  eta 35s    
15% [=============================>                                                                                                                                                                      ] 6,429,811   1.04MB/s  eta 35s    
16% [===============================>                                                                                                                                                                    ] 6,708,339   1.06MB/s  eta 35s    
16% [================================>                                                                                                                                                                   ] 6,904,947   1.05MB/s  eta 35s    
17% [=================================>                                                                                                                                                                  ] 7,167,091   1.08MB/s  eta 35s    
18% [==================================>                                                                                                                                                                 ] 7,380,083   1.06MB/s  eta 33s    
18% [===================================>                                                                                                                                                                ] 7,642,227   1.08MB/s  eta 33s    
19% [====================================>                                                                                                                                                               ] 7,855,219   1.07MB/s  eta 33s    
19% [=====================================>                                                                                                                                                              ] 8,133,747   1.08MB/s  eta 33s    
20% [======================================>                                                                                                                                                             ] 8,346,739   1.07MB/s  eta 33s    
21% [========================================>                                                                                                                                                           ] 8,625,267   1.09MB/s  eta 31s    
21% [=========================================>                                                                                                                                                          ] 8,838,259   1.09MB/s  eta 31s    
22% [==========================================>                                                                                                                                                         ] 9,116,787   1.08MB/s  eta 31s    
22% [===========================================>                                                                                                                                                        ] 9,329,779   1.08MB/s  eta 31s    
23% [=============================================>                                                                                                                                                      ] 9,624,691   1.10MB/s  eta 31s    
24% [==============================================>                                                                                                                                                     ] 9,837,683   1.10MB/s  eta 30s    
24% [===============================================>                                                                                                                                                    ] 10,132,595  1.11MB/s  eta 30s    
25% [================================================>                                                                                                                                                   ] 10,361,971  1.11MB/s  eta 30s    
26% [==================================================>                                                                                                                                                 ] 10,673,267  1.14MB/s  eta 30s    
26% [===================================================>                                                                                                                                                ] 10,919,027  1.14MB/s  eta 30s    
27% [====================================================>                                                                                                                                               ] 11,246,707  1.15MB/s  eta 28s    
28% [======================================================>                                                                                                                                             ] 11,492,467  1.16MB/s  eta 28s    
28% [=======================================================>                                                                                                                                            ] 11,852,915  1.20MB/s  eta 28s    
29% [=========================================================>                                                                                                                                          ] 12,115,059  1.21MB/s  eta 28s    
30% [==========================================================>                                                                                                                                         ] 12,491,891  1.23MB/s  eta 28s    
31% [============================================================>                                                                                                                                       ] 12,786,803  1.25MB/s  eta 25s    
32% [==============================================================>                                                                                                                                     ] 13,180,019  1.30MB/s  eta 25s    
32% [===============================================================>                                                                                                                                    ] 13,491,315  1.32MB/s  eta 25s    
34% [=================================================================>                                                                                                                                  ] 13,933,683  1.38MB/s  eta 25s    
34% [==================================================================>                                                                                                                                 ] 14,097,523  1.31MB/s  eta 25s    
35% [=====================================================================>                                                                                                                              ] 14,703,731  1.41MB/s  eta 23s    
36% [======================================================================>                                                                                                                             ] 14,998,643  1.42MB/s  eta 23s    
37% [========================================================================>                                                                                                                           ] 15,293,555  1.44MB/s  eta 23s    
38% [=========================================================================>                                                                                                                          ] 15,604,851  1.45MB/s  eta 23s    
38% [===========================================================================>                                                                                                                        ] 15,916,147  1.46MB/s  eta 23s    
39% [============================================================================>                                                                                                                       ] 16,243,827  1.48MB/s  eta 21s    
40% [==============================================================================>                                                                                                                     ] 16,587,891  1.50MB/s  eta 21s    
41% [================================================================================>                                                                                                                   ] 16,948,339  1.51MB/s  eta 21s    
42% [=================================================================================>                                                                                                                  ] 17,308,787  1.53MB/s  eta 21s    
43% [===================================================================================>                                                                                                                ] 17,685,619  1.54MB/s  eta 21s    
44% [=====================================================================================>                                                                                                              ] 18,062,451  1.57MB/s  eta 19s    
45% [=======================================================================================>                                                                                                            ] 18,439,283  1.57MB/s  eta 19s    
46% [=========================================================================================>                                                                                                          ] 18,840,691  1.59MB/s  eta 19s    
46% [==========================================================================================>                                                                                                         ] 19,192,947  1.59MB/s  eta 19s    
47% [============================================================================================>                                                                                                       ] 19,618,931  1.61MB/s  eta 19s    
48% [==============================================================================================>                                                                                                     ] 19,995,763  1.71MB/s  eta 16s    
49% [================================================================================================>                                                                                                   ] 20,421,747  1.72MB/s  eta 16s    
50% [==================================================================================================>                                                                                                 ] 20,798,579  1.69MB/s  eta 16s    
51% [====================================================================================================>                                                                                               ] 21,240,947  1.72MB/s  eta 16s    
52% [======================================================================================================>                                                                                             ] 21,617,779  1.74MB/s  eta 16s    
53% [========================================================================================================>                                                                                           ] 22,060,147  1.79MB/s  eta 14s    
54% [==========================================================================================================>                                                                                         ] 22,445,171  1.79MB/s  eta 14s    
55% [============================================================================================================>                                                                                       ] 22,879,347  1.81MB/s  eta 14s    
56% [==============================================================================================================>                                                                                     ] 23,256,179  1.82MB/s  eta 14s    
57% [================================================================================================================>                                                                                   ] 23,698,547  1.83MB/s  eta 14s    
58% [==================================================================================================================>                                                                                 ] 24,075,379  1.83MB/s  eta 12s    
59% [====================================================================================================================>                                                                               ] 24,534,131  1.85MB/s  eta 12s    
60% [======================================================================================================================>                                                                             ] 24,927,347  1.84MB/s  eta 12s    
61% [========================================================================================================================>                                                                           ] 25,369,715  1.87MB/s  eta 12s    
62% [==========================================================================================================================>                                                                         ] 25,746,547  1.86MB/s  eta 12s    
63% [============================================================================================================================>                                                                       ] 26,188,915  1.87MB/s  eta 11s    
64% [==============================================================================================================================>                                                                     ] 26,565,747  1.86MB/s  eta 11s    
65% [================================================================================================================================>                                                                   ] 27,008,115  1.87MB/s  eta 11s    
66% [==================================================================================================================================>                                                                 ] 27,384,947  1.86MB/s  eta 11s    
68% [====================================================================================================================================>                                                               ] 27,843,699  1.89MB/s  eta 11s    
68% [======================================================================================================================================>                                                             ] 28,220,531  1.87MB/s  eta 9s     
70% [========================================================================================================================================>                                                           ] 28,679,283  1.88MB/s  eta 9s     
70% [==========================================================================================================================================>                                                         ] 29,056,115  1.87MB/s  eta 9s     
72% [============================================================================================================================================>                                                       ] 29,514,867  1.89MB/s  eta 9s     
73% [==============================================================================================================================================>                                                     ] 29,908,083  1.88MB/s  eta 9s     
74% [================================================================================================================================================>                                                   ] 30,383,219  1.91MB/s  eta 7s     
75% [==================================================================================================================================================>                                                 ] 30,792,819  1.90MB/s  eta 7s     
76% [====================================================================================================================================================>                                               ] 31,284,339  1.92MB/s  eta 7s     
77% [======================================================================================================================================================>                                             ] 31,677,555  1.93MB/s  eta 7s     
78% [=========================================================================================================================================================>                                          ] 32,185,459  1.96MB/s  eta 7s     
79% [===========================================================================================================================================================>                                        ] 32,611,443  1.93MB/s  eta 6s     
80% [=============================================================================================================================================================>                                      ] 33,152,115  1.97MB/s  eta 6s     
82% [===============================================================================================================================================================>                                    ] 33,578,099  1.98MB/s  eta 6s     
83% [==================================================================================================================================================================>                                 ] 34,135,155  2.03MB/s  eta 6s     
84% [====================================================================================================================================================================>                               ] 34,577,523  2.04MB/s  eta 6s     
85% [=======================================================================================================================================================================>                            ] 35,167,347  2.09MB/s  eta 4s     
87% [=========================================================================================================================================================================>                          ] 35,642,483  2.11MB/s  eta 4s     
88% [============================================================================================================================================================================>                       ] 36,232,307  2.15MB/s  eta 4s     
89% [==============================================================================================================================================================================>                     ] 36,715,635  2.18MB/s  eta 4s     
90% [================================================================================================================================================================================>                   ] 36,969,587  2.09MB/s  eta 4s     
92% [====================================================================================================================================================================================>               ] 37,854,323  2.22MB/s  eta 2s     
93% [======================================================================================================================================================================================>             ] 38,296,691  2.22MB/s  eta 2s     
94% [========================================================================================================================================================================================>           ] 38,755,443  2.22MB/s  eta 2s     
95% [==========================================================================================================================================================================================>         ] 39,197,811  2.21MB/s  eta 2s     
96% [===========================================================================================================================================================================================>        ] 39,296,115  1.95MB/s  eta 1s     
96% [============================================================================================================================================================================================>       ] 39,591,027  1.87MB/s  eta 1s     
98% [===============================================================================================================================================================================================>    ] 40,279,155  1.86MB/s  eta 1s     
99% [==================================================================================================================================================================================================> ] 40,819,827  1.87MB/s  eta 1s     
100%[===================================================================================================================================================================================================>] 40,931,771  1.84MB/s   in 26s    

2023-05-23 07:06:01 (1.48 MB/s) - '/otus4/pg2600.converter.log' saved [40931771/40931771]

```
9. Проверяем степень сжатия в кажом пуле:

```
[root@zfs ~]# zfs list
NAME    USED  AVAIL     REFER  MOUNTPOINT
otus1  21.6M   330M     21.6M  /otus1
otus2  17.7M   334M     17.6M  /otus2
otus3  10.8M   341M     10.7M  /otus3
otus4  39.2M   313M     39.1M  /otus4
[root@zfs ~]# zfs get all | grep compressratio | grep -v ref
otus1  compressratio         1.81x                  -
otus2  compressratio         2.22x                  -
otus3  compressratio         3.65x                  -
otus4  compressratio         1.00x                  -
```

10. Скачиваем архив в домашний каталог

```
[root@zfs ~]# wget -O archive.tar.gz --no-check-certificate 'https://drive.google.com/u/0/uc?id=1KRBNW33QWqbvbVHa3hLJivOAt60yukkg&confirm=t&export=download'
--2023-05-23 07:09:20--  https://drive.google.com/u/0/uc?id=1KRBNW33QWqbvbVHa3hLJivOAt60yukkg&confirm=t&export=download
Resolving drive.google.com (drive.google.com)... 64.233.163.194, 2a00:1450:4010:c0b::c2
Connecting to drive.google.com (drive.google.com)|64.233.163.194|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://drive.google.com/uc?id=1KRBNW33QWqbvbVHa3hLJivOAt60yukkg&confirm=t&export=download [following]
--2023-05-23 07:09:20--  https://drive.google.com/uc?id=1KRBNW33QWqbvbVHa3hLJivOAt60yukkg&confirm=t&export=download
Reusing existing connection to drive.google.com:443.
HTTP request sent, awaiting response... 303 See Other
Location: https://doc-0c-bo-docs.googleusercontent.com/docs/securesc/ha0ro937gcuc7l7deffksulhg5h7mbp1/h6srual543d4mhpsd234cgc00k37dkej/1684825725000/16189157874053420687/*/1KRBNW33QWqbvbVHa3hLJivOAt60yukkg?e=download&uuid=21a2d60f-2888-4fb9-b0ef-27feb697fa91 [following]
Warning: wildcards not supported in HTTP.
--2023-05-23 07:09:27--  https://doc-0c-bo-docs.googleusercontent.com/docs/securesc/ha0ro937gcuc7l7deffksulhg5h7mbp1/h6srual543d4mhpsd234cgc00k37dkej/1684825725000/16189157874053420687/*/1KRBNW33QWqbvbVHa3hLJivOAt60yukkg?e=download&uuid=21a2d60f-2888-4fb9-b0ef-27feb697fa91
Resolving doc-0c-bo-docs.googleusercontent.com (doc-0c-bo-docs.googleusercontent.com)... 64.233.165.132, 2a00:1450:4010:c08::84
Connecting to doc-0c-bo-docs.googleusercontent.com (doc-0c-bo-docs.googleusercontent.com)|64.233.165.132|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 7275140 (6.9M) [application/x-gzip]
Saving to: 'archive.tar.gz'


 0% [                                                                                                                                                                                                    ] 0           --.-K/s              
 2% [===>                                                                                                                                                                                                ] 159,546      775KB/s             
17% [=================================>                                                                                                                                                                  ] 1,281,618   3.04MB/s             
27% [====================================================>                                                                                                                                               ] 1,986,019   2.75MB/s             
62% [=========================================================================================================================>                                                                          ] 4,562,882   4.90MB/s             
76% [====================================================================================================================================================>                                               ] 5,562,166   4.86MB/s             
100%[===================================================================================================================================================================================================>] 7,275,140   5.79MB/s   in 1.2s   

2023-05-23 07:09:29 (5.79 MB/s) - 'archive.tar.gz' saved [7275140/7275140]
```

11. Разархивируем

```
[root@zfs ~]# tar -xzvf archive.tar.gz
zpoolexport/
zpoolexport/filea
zpoolexport/fileb
```

12. Проверим, возможно ли импортировать данный каталог в пул

```
[root@zfs ~]# zpool import -d zpoolexport/
   pool: otus
     id: 6554193320433390805
  state: ONLINE
 action: The pool can be imported using its name or numeric identifier.
 config:

otus                         ONLINE
  mirror-0                   ONLINE
    /root/zpoolexport/filea  ONLINE
    /root/zpoolexport/fileb  ONLINE
```

13. Импортируем его в ОС и проверим статус

```
[root@zfs ~]# zpool import -d zpoolexport/ otus
[root@zfs ~]# zpool status
  pool: otus
 state: ONLINE
  scan: none requested
config:

NAME                         STATE     READ WRITE CKSUM
otus                         ONLINE       0     0     0
  mirror-0                   ONLINE       0     0     0
    /root/zpoolexport/filea  ONLINE       0     0     0
    /root/zpoolexport/fileb  ONLINE       0     0     0

errors: No known data errors
 pool: otus1
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus1       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdb     ONLINE       0     0     0
    sdc     ONLINE       0     0     0

errors: No known data errors

  pool: otus2
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus2       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdd     ONLINE       0     0     0
    sde     ONLINE       0     0     0

errors: No known data errors

  pool: otus3
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus3       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdf     ONLINE       0     0     0
    sdg     ONLINE       0     0     0

errors: No known data errors

  pool: otus4
 state: ONLINE
  scan: none requested
config:

NAME        STATE     READ WRITE CKSUM
otus4       ONLINE       0     0     0
  mirror-0  ONLINE       0     0     0
    sdh     ONLINE       0     0     0
    sdi     ONLINE       0     0     0

errors: No known data errors
```

14. Смотрим все настройки пула otus

```
[root@zfs ~]# zpool get all otus
NAME  PROPERTY                       VALUE                          SOURCE
otus  size                           480M                           -
otus  capacity                       0%                             -
otus  altroot                        -                              default
otus  health                         ONLINE                         -
otus  guid                           6554193320433390805            -
otus  version                        -                              default
otus  bootfs                         -                              default
otus  delegation                     on                             default
otus  autoreplace                    off                            default
otus  cachefile                      -                              default
otus  failmode                       wait                           default
otus  listsnapshots                  off                            default
otus  autoexpand                     off                            default
otus  dedupditto                     0                              default
otus  dedupratio                     1.00x                          -
otus  free                           478M                           -
otus  allocated                      2.09M                          -
otus  readonly                       off                            -
otus  ashift                         0                              default
otus  comment                        -                              default
otus  expandsize                     -                              -
otus  freeing                        0                              -
otus  fragmentation                  0%                             -
otus  leaked                         0                              -
otus  multihost                      off                            default
otus  checkpoint                     -                              -
otus  load_guid                      17386143810256873327           -
otus  autotrim                       off                            default
otus  feature@async_destroy          enabled                        local
otus  feature@empty_bpobj            active                         local
otus  feature@lz4_compress           active                         local
otus  feature@multi_vdev_crash_dump  enabled                        local
otus  feature@spacemap_histogram     active                         local
otus  feature@enabled_txg            active                         local
otus  feature@hole_birth             active                         local
otus  feature@extensible_dataset     active                         local
otus  feature@embedded_data          active                         local
otus  feature@bookmarks              enabled                        local
otus  feature@filesystem_limits      enabled                        local
otus  feature@large_blocks           enabled                        local
otus  feature@large_dnode            enabled                        local
otus  feature@sha512                 enabled                        local
otus  feature@skein                  enabled                        local
otus  feature@edonr                  enabled                        local
otus  feature@userobj_accounting     active                         local
otus  feature@encryption             enabled                        local
otus  feature@project_quota          active                         local
otus  feature@device_removal         enabled                        local
otus  feature@obsolete_counts        enabled                        local
otus  feature@zpool_checkpoint       enabled                        local
otus  feature@spacemap_v2            active                         local
otus  feature@allocation_classes     enabled                        local
otus  feature@resilver_defer         enabled                        local
otus  feature@bookmark_v2            enabled                        local
```

15. Делаем выборку настроек пула по конкретным параметрам

```
[root@zfs ~]# zfs get available otus
NAME  PROPERTY   VALUE  SOURCE
otus  available  350M   -
[root@zfs ~]# zfs get readonly otus
NAME  PROPERTY  VALUE   SOURCE
otus  readonly  off     default
[root@zfs ~]# zfs get recordsize otus
NAME  PROPERTY    VALUE    SOURCE
otus  recordsize  128K     local
[root@zfs ~]# zfs get compression otus
NAME  PROPERTY     VALUE     SOURCE
otus  compression  zle       local
[root@zfs ~]# zfs get checksum otus
NAME  PROPERTY  VALUE      SOURCE
otus  checksum  sha256     local
```

16. Качаем файл из задания:

```
[root@zfs ~]# wget -O otus_task2.file --no-check-certificate 'https://drive.google.com/u/0/uc?id=1gH8gCL9y7Nd5Ti3IRmplZPF1XjzxeRAG&confirm=t&export=download'
--2023-05-23 07:34:13--  https://drive.google.com/u/0/uc?id=1gH8gCL9y7Nd5Ti3IRmplZPF1XjzxeRAG&confirm=t&export=download
Resolving drive.google.com (drive.google.com)... 173.194.222.194, 2a00:1450:4010:c0b::c2
Connecting to drive.google.com (drive.google.com)|173.194.222.194|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://drive.google.com/uc?id=1gH8gCL9y7Nd5Ti3IRmplZPF1XjzxeRAG&confirm=t&export=download [following]
--2023-05-23 07:34:13--  https://drive.google.com/uc?id=1gH8gCL9y7Nd5Ti3IRmplZPF1XjzxeRAG&confirm=t&export=download
Reusing existing connection to drive.google.com:443.
HTTP request sent, awaiting response... 303 See Other
Location: https://doc-00-bo-docs.googleusercontent.com/docs/securesc/ha0ro937gcuc7l7deffksulhg5h7mbp1/ug50349fsmp5o7j7ansgba9ognqdc65e/1684827225000/16189157874053420687/*/1gH8gCL9y7Nd5Ti3IRmplZPF1XjzxeRAG?e=download&uuid=739d6526-2c15-4078-924d-58b192946434 [following]
Warning: wildcards not supported in HTTP.
--2023-05-23 07:34:17--  https://doc-00-bo-docs.googleusercontent.com/docs/securesc/ha0ro937gcuc7l7deffksulhg5h7mbp1/ug50349fsmp5o7j7ansgba9ognqdc65e/1684827225000/16189157874053420687/*/1gH8gCL9y7Nd5Ti3IRmplZPF1XjzxeRAG?e=download&uuid=739d6526-2c15-4078-924d-58b192946434
Resolving doc-00-bo-docs.googleusercontent.com (doc-00-bo-docs.googleusercontent.com)... 64.233.165.132, 2a00:1450:4010:c08::84
Connecting to doc-00-bo-docs.googleusercontent.com (doc-00-bo-docs.googleusercontent.com)|64.233.165.132|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 5432736 (5.2M) [application/octet-stream]
Saving to: 'otus_task2.file'


 0% [                                                                                                                                                                                                    ] 0           --.-K/s              
 2% [====>                                                                                                                                                                                               ] 151,284      733KB/s             
23% [=============================================>                                                                                                                                                      ] 1,277,338   3.03MB/s             
27% [=====================================================>                                                                                                                                              ] 1,502,289   2.32MB/s             
53% [========================================================================================================>                                                                                           ] 2,920,122   3.41MB/s             
97% [==============================================================================================================================================================================================>     ] 5,295,795   4.86MB/s             
100%[===================================================================================================================================================================================================>] 5,432,736   4.98MB/s   in 1.0s   

2023-05-23 07:34:18 (4.98 MB/s) - 'otus_task2.file' saved [5432736/5432736]
```

17. Восстановим файловую систему из снапшота

```
[root@zfs ~]# zfs receive otus/test@today < otus_task2.file
```

18. Находим в каталоге /otus/test файл с именем “secret_message” и смотрим его содержимое
 
```
[root@zfs test]# find /otus/test -name "secret_message"
/otus/test/task1/file_mess/secret_message
[root@zfs test]# cat /otus/test/task1/file_mess/secret_message
https://github.com/sindresorhus/awesome
```



