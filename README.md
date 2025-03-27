HOW TO PATCH
------------------------

- generate a generic entitlements.xml 

- Delete /Applications/IDA Professional 9.0 .app/Contents/MacOS/plugins/arm_mac_user64.dylib; python script.py

- delete the old dylibs, rename the new one's;

- run: codesign --sign - --entitlements entitlements.xml --force libida.dylib

- run: codesign --sign - --entitlements entitlements.xml --force libida64.dylib


------------------------

  or as the original poster said:

1. edit license owner and stuff to whatever you want
2. place ida/ida64 dll/so/dylib in same dir as script
3. run the script to generate a license
4. copy the generated license and replace dlls with patched ones
5. run and activate it lol
   
------------------------
magnet link

magnet:?xt=urn:btih:029e7eeb23e1a0f5b8b9a9269266bb74440498f6&xt=urn:btmh:12203f7a9a613035ab8921fb8eeab920a02d56114606c9aceb41e62bfbb9d355543b&dn=IDA%20Pro%209.0&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce&tr=udp%3A%2F%2Fopen.tracker.cl%3A1337%2Fannounce&tr=udp%3A%2F%2Fopen.demonii.com%3A1337%2Fannounce&tr=udp%3A%2F%2Fopen.stealth.si%3A80%2Fannounce&tr=udp%3A%2F%2Fexodus.desync.com%3A6969%2Fannounce&tr=udp%3A%2F%2Fopentracker.io%3A6969%2Fannounce&tr=udp%3A%2F%2Fnew-line.net%3A6969%2Fannounce&tr=udp%3A%2F%2Fexplodie.org%3A6969%2Fannounce&tr=udp%3A%2F%2Fepider.me%3A6969%2Fannounce&tr=udp%3A%2F%2Fbt1.archive.org%3A6969%2Fannounce

------------------------

original poster
https://gist.github.com/gmh5225/ddac451f209afdcc8e7aea94fe7d7c92
