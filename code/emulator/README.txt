Android 2.1 Emulator ʹ�÷���
=====================================================================================
����ѹѹ������ѹ���D:\AndroidEmulatorĿ¼��

1. ����ģ��������cmd����ڣ����뵽D:\AndroidEmulatorĿ¼��ִ���������
D:\AndroidEmulator>start /b emulator.exe -sysdir d:\AndroidEmulator -system images\system.img -data images\userdata.img -ramdisk images\ramdisk.img -kernel images\kernel-qemu -skindir d:\AndroidEmulator\skins -skin HVGA
      
2. ����ʾ������ִ������
D:\AndroidEmulator>adb install Renju\Renju.apk
����������������
* daemon not running. starting it now on port 5037 *
* daemon started successfully *
error: device offline
������ᣬ����ִ��adb install Renju\Renju.apk����ɡ�

ģ������������������ο�������߸��˲������£�http://blog.csdn.net/luoshengyang/article/details/6586759
ʾ������Renju.apk��һ������ʽ�˻���ս��������Ϸ������Ȥ��ο�RenjuĿ¼�µ�ʹ��˵�������߹�ע���˲��ͣ�http://blog.csdn.net/luoshengyang


Android 2.1 Emulator ��������
======================================================================================
 ������Ǳ�д��һ��AndroidӦ�ó�������һ̨û��Android SDK����BUILD�����Ļ�����ʾ�����˿���Ӧ����ô���أ�ͨ�������ǿ���AndroidӦ�ó����ʱ�򣬶���ʹ��ģ���������г���Ҫô��SDK�����£�Ҫô����Դ����BUILD������ʹ�á���SDK�����£����Eclipse��ADT��ʹ��ģ�����ܷ��㣬��BUILD�����£�Ҳ�Ǻܼ򵥵�ʹ��emulator����Ϳ����ˣ�������Բο���Ubuntu�����ء�����Ͱ�װAndroid����Դ����һ�ġ���ƪ���½�������һ�ַ�����Windows�»�����ʹ��Androidģ����������������SDK����BUILD���������Զ����ַ���ʹ�á�

Ҫ����Androidģ����emulator��ֻҪ�߱�4��ϵͳ����Ϳ����ˣ��ֱ���system.img��userdata.img��ramdisk.img��kernel-qemu����4���ļ��������ڴ�SDK�����еõ������⣬��û�Ҫ���ģ����Ƥ����adb���ߣ��������ܲ������������½��ܾ����Ʒ�����

һ. ����Android SDK���ٷ�����http://dl.google.com/android/android-sdk_rXX-windows.zip��XX��ָ��Ҫ���صİ汾�ţ����������ص���08�������ӿ����Ѿ�����г������������������һ�£��������취���ء����غ�֮������SDK Manager���ߣ�����������SDK������SDK����D:\android-sdk-windowsĿ¼�¡�

��. �½�һ��Ŀ¼�����磬��D�����½�Ŀ¼D:\AndroidEmulator�����뵽D:\android-sdk-windows\toolsĿ¼�£���emulator.exe��������D:\AndroidEmulator�У�ͬʱ���뵽D:\android-sdk-windows\platform-toolsĿ¼�£�����adb.exe��AdbWinApi.dll�����ļ���D:\AndroidEmulator�С�ע�⣬�е�SDK��adb.exe��AdbWinApi.dll����D:\android-sdk-windows\toolsĿ¼�¡�

��. ��D:\AndroidEmulator�½�Ŀ¼images��������������ᵽ��4��ϵͳ��������Ҫ����Android2.1ģ��������D:\android-sdk-windows\platforms\android-7\imagesĿ¼�£���������ļ�ȫ��������D:\AndroidEmulator\imagesĿ¼�£�D:\android-sdk-windows\platforms\android-7\imagesĿ¼������system.img��userdata.img��ramdisk.img��kernel-qemu��4���ļ���

��. ��D:\AndroidEmulator�½�Ŀ¼skins���������ģ����Ƥ���ļ�������������Android2.1ģ����Ϊ������D:\android-sdk-windows\platforms\android-7\skinsĿ¼�£����������е��ļ��п�����D:\AndroidEmulator\skinsĿ¼�£�D:\android-sdk-windows\platforms\android-7\skinsĿ¼������ģ����Ƥ���ļ���

��. ���������д��ڣ����뵽D:\AndroidEmulatorĿ¼��ִ���������

D:\AndroidEmulator>start /b emulator.exe -sysdir d:\AndroidEmulator -system images\system.img -data images\userdata.img -ramdisk images\ramdisk.img -kernel images\kernel-qemu -skindir d:\AndroidEmulator\skins -skin HVGA

start /b��ʾ�ں�̨����emulator������emulator����ѡ����ִ��emulator -help�鿴��������ģ�������������ˡ�

��. ���Ҫ��ģ�����ϰ�װAPK������ִ��adb install XXX.apk�������adb install����ʱ������������������

D:\AndroidEmulator>adb install Renju.apk
* daemon not running. starting it now on port 5037 *
* daemon started successfully *
error: device offline

������ᣬ�������У�ֱ����ʾ�ɹ�Ϊֹ��

������������Ǳ�д��һ��AndroidӦ�ó������õ�һ̨û��Android SDK��Android Build�����Ļ�������ʾ�����˿����Ϳ��Դ��D:\AndroidEmulator����ļ��У��ٴ������AndroidӦ�ó��򣬾Ϳ�����ʾ�ˣ��ǲ��Ǻܷ����ء�