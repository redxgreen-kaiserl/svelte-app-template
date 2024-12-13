1. npm install
2. npx cap add ios
3. ios/App/Podfile => delete # workaround to avoid Xcode caching of Pods that requires
                             # Product -> Clean Build Folder after new Cordova plugins installed
                             # Requires CocoaPods 1.6 or newer
                             install! 'cocoapods', :disable_input_output_paths => true
4. npx cap run ios

# deployment
1. npm run build
2. capacitor.config.ts => delete URL
3. npx cap add ios
