# log4j-rce-fix-patched-jars CVE-2021-44228
Here you find all log4j version jars recompiled with the lookup function returning null. this is for those who have no updates, can not upgrade their applications or dependencies.

example for exchanging a log4j-core jar in your app.
1. cp target.mar /tmp/
2. jar xvf target.mar 
3. replace your log4j-core-x.xx.jar with the patched one (remove patched from patched filename so it matches the original one)
4. jar cvfm target.mar MANIFEST/MANIFEST.MF *
5. copy back the new target.mar into your application and replace old file.
