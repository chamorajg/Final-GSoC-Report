# Final-GSoC-Report
***
---
## GSoC report of Chandramouli Rajagopalan under Debian Android Tools
***
---
# [Android-platfrom-external-libselinux](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-libselinux)
* [Update selinux to libselinux from AOSP to new upstream version 8.1.0+r23](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-libselinux)
* [Updated makefile in libselinux](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-libselinux/commit/6a2e029933f50e22049d96446e7cfa130eb1852c#71c7a7875a21c214a3cd22172642c6e627918ae4)
* [Updated the changelog to include the new upstream version change](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-libselinux/commit/6a2e029933f50e22049d96446e7cfa130eb1852c#9c96da0e9f91d7d8937b69b524702c106258f0d1)
* [Included myself in the Uploaders list for the package](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-libselinux/commit/6a2e029933f50e22049d96446e7cfa130eb1852c#58ef006ab62b83b4bec5d81fe5b32c3b4c2d1cc2)
* [Updated rules file](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-libselinux/commit/6a2e029933f50e22049d96446e7cfa130eb1852c#8756c63497c8dc39f7773438edf53b220c773f67)
***
---
# [Android-platform-external-boringssl](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl)	
* [New Package boringssl has been uploaded to replace openssl to include only binaries required by AOSP](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl)
* [Updated boringssl install file](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#5351a44a0faaf983f656ec1d5dd3adc8f03a4ddd)
* [Updated boringssl docs file](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#f46f370a3984c30af8dd8e2e6cef80b819306351)
* [Updated debian control file to include make instead of cmake](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#58ef006ab62b83b4bec5d81fe5b32c3b4c2d1cc2)
* [Created a detect arch makefile to detect architecture of the target](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#cd2aeb4ab668ea0f0b625546c63384722c4e01c6) 
* [Created libcrypto makefile for libcrypto binary](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#f8e8fe159442ea71a9de9f76f4072c1c29812428) 
* [Created libssl makefile for libssl binary](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#188c53015950adda2aa8c131f2e22c36e43e574f) 
* [Updated rules file to build with make instead of cmake](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/37485f76ca74c196bdac69680bba64af6551712d#8756c63497c8dc39f7773438edf53b220c773f67) 
* [Updated control to update all build dependencies](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/3e5286e3eefc37bf6ddf88c88c8c10d4cbac285b#78fd675df1cf8c2d4c62ae1a9a912d15c8c50ba4) 
* [Updated copyright files to include updated files and exclude outdated information](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/3e5286e3eefc37bf6ddf88c88c8c10d4cbac285b#adb7f75f79e3bb85eb62912a2904c5d24af878fb)
* [Removed lintian warnings and reduced it to minimum](https://salsa.debian.org/r_chandramouli-guest/android-platform-external-boringssl/commit/3e5286e3eefc37bf6ddf88c88c8c10d4cbac285b)
***
---
# [Android-platform-system-core](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core)
* [Updated libadb install to include changes](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/0d44234489c723d72ad9a152fce1c067ebff1e9a)
* [Updated libcrypto_utils install](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/0d44234489c723d72ad9a152fce1c067ebff1e9a#ab9d06f11593cf4cbedb827a5f2f1d0545a4e43e) 
* [Updated rules to overcome shlibs error](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/615256da501893dfbd7db907a17fdb39a2a43774#8756c63497c8dc39f7773438edf53b220c773f67)
* [Updated abd makefile](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/58d0eb686d63596a1b84910b3d8f39c3bcddf0cd#134e3786b2d7c796cecab235de509a4849b9b29a)
* [Updated simg2simg makefile](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/2b807bd7509a0ca16ffb679ac43b1fc4493ba7dd)
* [Updated libziparchive to include required files from libziparchive directory](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/2b23570a3c6a36b7a7184e5fc0d50e09c8a6d53a)
* [Included utils.patch in series](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/ee37adc57213711166a466ef4456f8c48cb4a60e)
* [Updated libutils to include inner libraries](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/72d3778335a0d640cd6adad1392214cd156faabe)
* [Updated libbacktrace to include req files](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/2d0e7f153aad0e75240a2d09b1151b35ed9352fa)
* [Updated append2simg makefile to include shared libraries](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/bfa74f51e39182538aa43ed3149fdcd0b240a725)
* [Updated img2simg to include shared libraries](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/7fd79b4b5552ea06111fc15356c1b2f572e1087d) 
* [Updated simg2simg to include shared libraries](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/19bcacff8f506b81048071ae51a436191296a002)
* [Created a patch to include C++ library version of library](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/cf9f229c7e80de66fd922e4b21de51289ac2dd70)
* [Included required libraries](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/ba4c543e6881f3b608402b31d0dea00813eabb3d)
* [Included libraries](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/35d897951eaf47f46194ddd53a405187c05e0f0e)
* [Defined extern to declare libraries according to compiler environment](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/4e34559fe684f15a437fd05092295533345a9d66)
* [Included libraries for fs_config](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/839802df45c2a650f51b3092b3c8e0c8bdca9dd6)
* [Update adb.patch](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/commit/75910392213966e8aec2e8c15f8aa8298b8f575a)
* [Changed variable name to prevent name conflicts](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/blob/master/debian/patches/backtraceh.patch)
* [Include C++ version of string library](https://salsa.debian.org/r_chandramouli-guest/android-platform-system-core/blob/master/debian/patches/errors_unix.patch)
***
---
# [Android-platform-libnativehelper](https://salsa.debian.org/r_chandramouli-guest/android-platform-libnativehelper)
* [Updated control file to change build dependencies as latest version of them are still need to be uploaded](https://salsa.debian.org/r_chandramouli-guest/android-platform-libnativehelper/commit/dacf17a05b1b09007713a3ea9d19b6fc36d82f73#58ef006ab62b83b4bec5d81fe5b32c3b4c2d1cc2)
* [Created libnativehelper makefile to create the binary files](https://salsa.debian.org/r_chandramouli-guest/android-platform-libnativehelper/commit/dacf17a05b1b09007713a3ea9d19b6fc36d82f73#adb7f75f79e3bb85eb62912a2904c5d24af878fb)
* [Included a patch to fix library conflicts](https://salsa.debian.org/r_chandramouli-guest/android-platform-libnativehelper/commit/dacf17a05b1b09007713a3ea9d19b6fc36d82f73#8b75bd278605686e12fd007a06004d16c03417d1)
* [Lintian warnings reduced](https://salsa.debian.org/r_chandramouli-guest/android-platform-libnativehelper/commit/dacf17a05b1b09007713a3ea9d19b6fc36d82f73#adb7f75f79e3bb85eb62912a2904c5d24af878fb)
***
---
# [Android-platform-libcore](https://salsa.debian.org/r_chandramouli-guest/android-platform-libcore)
* [Created gitlab.yml file for CI tests](https://salsa.debian.org/r_chandramouli-guest/android-platform-libcore/commit/b4f375c659b76bd5d89b0c5380850b8672f50745)
*** 
---
# [Dummydroid](https://salsa.debian.org/r_chandramouli-guest/dummydroid)
* [Updated the git and browser link in the control file](https://salsa.debian.org/r_chandramouli-guest/dummydroid/commit/be44a89dc060337d61ef610dd667db8991665a47)
* [Updated the dependancy issue. Junit has been included as a dependancy](https://salsa.debian.org/r_chandramouli-guest/dummydroid/commit/496d46296d426bf3c984639d40c31838c73547d3)
* [Created and Updated gitlab.yml file for CI tests](https://salsa.debian.org/r_chandramouli-guest/dummydroid/commit/11ef213e27eae7cd24116f77a5a79441e4947dd1)
***
---
# [Libscout](https://salsa.debian.org/r_chandramouli-guest/libscout)
* [Issues were present with the source code, So created an issue in the github repository.](https://github.com/reddr/LibScout/issues/16)(The package has error in it’s source code. So cannot complete building unless the source code is fixed.)
***
---
# [Android-platform-frameworks-compile-libbcc](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-libbcc)(Currently Working)
* [Included the new upstream version (8.1.0+r23) in the changelog](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-libbcc/commit/1c11a64a08633f739078acf5dbc825ece4087e46#9c96da0e9f91d7d8937b69b524702c106258f0d1)
* [Created bcc makefile for binary file](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-libbcc/commit/1c11a64a08633f739078acf5dbc825ece4087e46#e98b3a8a3cad0322001ad1efef6159286b9116b8)
* [Created bcc_compat makefile for binary](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-libbcc/commit/1c11a64a08633f739078acf5dbc825ece4087e46#11db5792e987621a95c76f812c1b9ea002c7d627)
* [Created libbcc makefile for binaries](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-libbcc/commit/1c11a64a08633f739078acf5dbc825ece4087e46#9c96da0e9f91d7d8937b69b524702c106258f0d1)
***
---
# [Android-platform-frameworks-compile-slang](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang)(Currently Working)
* [Created libslang makefile required for binaries](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang/commit/a83ab5b7428663be54f69f8f6e3a0860afe9e1d8#3390de9e28675953bcb4c677ab02afbef65f0ad7)
* [Included the new upstream version in changelog (8.1.0+r23)](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang/commit/a83ab5b7428663be54f69f8f6e3a0860afe9e1d8#9c96da0e9f91d7d8937b69b524702c106258f0d1)
* [Included libwriter_3_2 as required by binaries](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang/commit/a83ab5b7428663be54f69f8f6e3a0860afe9e1d8#8ab68b068ec7aac9e16502be94d55492ccfd33e7)
* [Created libstripunkattr makefile](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang/commit/a83ab5b7428663be54f69f8f6e3a0860afe9e1d8#29e554491c7cabe8dcdb96b17e8075b220bdefa1)
* [Created libwriter_2_9 makefile](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang/commit/a83ab5b7428663be54f69f8f6e3a0860afe9e1d8#e405245abe3ca2132846d5dd91e4509612d224ae)
* [Created libwriter_2_9_func makefile](https://salsa.debian.org/r_chandramouli-guest/android-platform-frameworks-compile-slang/commit/a83ab5b7428663be54f69f8f6e3a0860afe9e1d8#8ab68b068ec7aac9e16502be94d55492ccfd33e7)
***
---
# [Android-parser](https://salsa.debian.org/r_chandramouli-guest/android-parser)(New Parser that parses .bp file to create makefiles)
* [Included the blueprint pareser and made changes to parse the input files to produce json file as output](https://salsa.debian.org/r_chandramouli-guest/android-parser/blob/6d9f4bf9ba856dfc26c1058e0d3ac3103986fbb1/bpfmt)
* [The python file takes json file as an input parses it and produces the makefile for Debian packaging](https://salsa.debian.org/r_chandramouli-guest/android-parser/commit/6d9f4bf9ba856dfc26c1058e0d3ac3103986fbb1#0406e50cd2538934c0bb2600061009037e0efbc2)
* [Created readme file for the parser](https://salsa.debian.org/r_chandramouli-guest/android-parser/commit/55d37cd1b729515dd9f28e6c234b2172e23d9281)
***
---
# My GSoC weekly report links can be found here :-
* [My GSoC weekly report for week 1](https://lists.debian.org/debian-outreach/2018/05/msg00022.html)
* [My GSoC weekly report for week 2](https://lists.debian.org/debian-outreach/2018/06/msg00023.html)
* [My GSoC weekly report for week 3](https://lists.debian.org/debian-outreach/2018/06/msg00024.html)
* [My GSoC weekly report for week 4](https://lists.debian.org/debian-outreach/2018/06/msg00069.html)
* [My GSoC weekly report for week 5](https://lists.debian.org/debian-outreach/2018/06/msg00088.html)
* [My GSoC weekly report for week 6](https://lists.debian.org/debian-outreach/2018/07/msg00015.html)
* [My GSoC weekly report for week 7](https://lists.debian.org/debian-outreach/2018/07/msg00014.html)
* [My GSoC weekly report for week 8](https://lists.debian.org/debian-outreach/2018/07/msg00029.html)
* [My GSoC weekly report for week 9](https://lists.debian.org/debian-outreach/2018/07/msg00083.html)
* [My GSoC weekly report for week 10](https://lists.debian.org/debian-outreach/2018/07/msg00084.html)
* [My GSoC weekly report for week 11](https://lists.debian.org/debian-outreach/2018/07/msg00109.html)
* [My GSoC weekly report for week 12](https://lists.debian.org/debian-outreach/2018/08/msg00056.html)
***
