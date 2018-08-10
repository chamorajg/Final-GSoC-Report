# Final-GSoC-Report
***
---
## GSoC report of Chandramouli Rajagopalan under Debian Android Tools
***
---
# Final GSoC Report Summary :-
This GSoC report  contains the summary of all the work I did during the past three months. First of all I would like to thank the Debian community , my mentors and Google for giving me this wonderful opportunity. Diving further into the project , I have started my project by updating packages which were of Stage 1(Packages were divided into four stages based on their requirement by other packages.) and then developing a parser that helps build makefiles for packaging and then updating other required packages.
You can always find me on #debian-mobile as chandramouli_r(through matrix) and on #debian-java with the same username mentioned above.
My gitlab account is https://salsa.debian.org/r_chandramouli-guest. You can find all my activities and forks of project that I have undertaken.
***
---
# Open Source - Software , GSoC and Debian :-
I would like to give a small description about open source and how it actually changed the  way I code. Open source software is a free distributed software where the owner of the software grants permission to change and distribute the software to anyone for any purpose. I got to know about open source software and contributing to open source when I applied for GSoC 2017. I got rejected last year and wanted to contribute again under the
same platform this year. I completed small tasks that were mentioned in the project page as an assignment to evaluate students before selecting the students. I would like to give Google the credit for this program as it has given all the students a chance to contribute to open source and to work under mentors who are highly qualified and for providing us this wonderful three months. I would want them to continue this initiative as it would help students understand how things work in reality.  And finally Debian, working with Debian environment and learning to package software has been great. I have been using Ubuntu from the past 3-4 years so I find Linux environment the best place for open source. Since Ubuntu being a Debian based distro where the packaging style is similar, I thought of contributing to Debian under Android-Tools as I was more familiar with android environment and the coding languages used. Talking about Debian environment, Debian mentors and the organisation has been the best and the people at debian have been receiving contributors in the best way possible. I would like to give the credit for my work to all the three mentors who have supported me from the beginning and patiently bearing with me throughout. Hans-Christoph-Steiner,Kai-Chung-Yan and Chirayu Desai you people have been the best and guided us so well to come up to this stage. I believe interaction with mentors is the most important aspect of GSoC where students get to learn work and contribute to the open source environment. Hans-Christoph-Steiner , Kai-
Chung-Yun and Chirayu Desai you guys deserve a big cheer for you work towards Debian. You guys have inspired us to keep contributing inspite of GSoC getting over.
***
---
# Android-Tools and My Work :-
I have started my work with packaging Stage 1 components (Android-platform-external-libselinux) . The packages have been divided into 4 sub categories such that the higher levels depend on the lower ones for updating. So we started out work with stage 1 components. After updating Android-platform-external-libselinux I started my work on Android-parser which parses .bp file to create makefiles by using blueprint convertor.Our mentors have figured out a way to update the package in a planned manner inorder to reduce the dependancy issues that might arise.
* Stage 1
  * android-framework-$apilevel
  * android-platform-external-jsilver (Usually no update needed)
  * android-platform-external-libselinux (should be switched to android-platform-external-selinux from 8.0 release)
  * android-platform-external-libunwind
  * android-platform-frameworks-data-binding
  * android-platform-frameworks-native
  * android-platform-libcore
  * android-platform-tools-analytics-library
* Stage 2
  * android-platform-external-doclava
  * android-platform-system-core~stage1
  * android-platform-tools-base
* Stage 3
  * android-platform-development
  * android-platform-frameworks-base
  * android-platform-libnativehelper
  * android-platform-system-extras
  * android-platform-system-tools-aidl
* Stage 4
  * android-platform-build
  * android-platform-dalvik
  * android-platform-system-core
* android-platform-dalvik (Needs android.jar of the latest API Level)

Then I got to update more packages like libscout , apktools and dummydroid. We introduced a new package android-platform-external-boringssl which is a part of OpenSSL but contains only files required by all the remaining android-* packages. And after that I continued my work on updating android-platform-libnativehelper, android-platfrom-system-core, and adding CI Tests to android-platform-libcore and finally dummydroid.
* Commits that have been merged :- 
 1. Android-platform-external-libselinux
 2. Android-platform-external-boringssl
* Commits yet to be merged :-
 3. Android-platform-system-core
 4. Android-platform-libnativehelper
 5. Android-platform-libcore
 6. dummydroid
 7. libscout
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
---
# Current Work and Future Contributions :-
I am now currently working on android-platform-frameworks-compile where my mentors have suggested me to divide the package into two :-
1.android-platform-frameworks-compile-libbcc
2.android-platform-frameworks-compile-slang
So I am now working on resolving the circular dependency between the two and updating them simulataneously. I currently have Job placement exams going on in my university from the past one week , So I couldn’t focus more towards my work as I was preparing for it. I have reported this issue to my mentors. As soon as the exams get over I would like to complete frameworks-compile and all the remaining packages to be packaged before finally updating to android version P. I would like to contribute to debian irrespective of this program. I would like to continue my work with debian for a long time from now. 
Thank You GSoC for this opportunity and Thank you mentors (Kai-Chung-Yun, Hans-Christoph-Steiner and Chirayu Desai) and Thanks Debian for this wonderful three months.

# Happy Open Sourcing :)
***
