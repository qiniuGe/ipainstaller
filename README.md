IPA Installer Console
=============

1 Mac电脑提前安装好theos;  

2 download工程，解压 cd ipainstaller-master;  

3 make package 完成后在该目录多出packages文件夹，deb在里面;  

4 ssh连接越狱机:  

ssh root@192.168.2.123   

alpine  

5 deb copy到越狱机var/root目录下;  

6 iPhone:~ root# dpkg -i com.autopear.installipa_3.4.1-1+debug_iphoneos-arm.deb,执行成功越狱机路径下出现：/usr/bin/installipa;  

7 测试：iPhone:~ root# installipa /var/mobile/Applications/4476654971728285.ipa.





[Update] This works for iOS 14.3.

Extract IPA using -B option

-----------------------------------
Requires iOS 4.0 or above

Check the releases page for the deb file. This was tested working on iOS 13.5 for arm64 devices.
arm7 devices are not supported (rather, arm7 was not a compilation target)

ZipArchive from https://github.com/mattconnolly/ZipArchive

UIDevice-Extension from https://github.com/erica/uidevice-extension

New check capability method from https://github.com/a3tweaks/Flipswitch/blob/master/FSCapability.m

MiniZip from http://www.winimage.com/zLibDll/minizip.html

fixblankicon is an executable from ipod4g, which is used in old script to fix blank icons. It is not used in the binary.

