# Cordova Firebase Example

This project is to provide an example of the cordova-firebasex plugin not building against an arm64 architecture mac

Steps to reproduce

1. Clone repository
2. `npm install`
3. `npx cordova prepare`
4. `npx cordova build ios`

What we should see in the build output is
```
ld: in [REDACTED]/platforms/ios/Pods/GoogleSymbolUtilities/Frameworks/frameworks/GoogleSymbolUtilities.framework/GoogleSymbolUtilities(overload.o), building for iOS Simulator, but linking in object file built for iOS, file '[REDACTED]/platforms/ios/Pods/GoogleSymbolUtilities/Frameworks/frameworks/GoogleSymbolUtilities.framework/GoogleSymbolUtilities' for architecture arm64
```
