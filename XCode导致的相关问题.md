# App Installation failed, No code signature found.
 - Solution:
  1. GO To "/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk"
  2. Open file SDKSettings.plist and check value for CODE_SIGNING_REQUIRED. If it is set 'NO' then set it 'YES'.
  3. Now relaunch the XCode. If it does not work again, then clear XCode DerivedData folder.
# 查找block中使用的self
 [参考](https://github.com/iteatimeteam/Friday-QA/issues/15)
 ```
 \^(\s*\(.*\)\s*)?\{(.|\n)*?\bself\b[^}]*\}
 ```
