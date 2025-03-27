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
