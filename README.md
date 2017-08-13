react-native unlink react-native-mfp && react-native uninstall react-native-mfp && npm uninstall --save react-native-mfp && npm install --save "../react-native-mfp" && react-native link

cd android && gradlew installDebug && cd ../
cd android && gradlew clean && cd ../

create mfpclient.properties file in android/app/src/main/assets
wlServerProtocol=http
wlServerHost=localhost
wlServerPort=9080
wlServerContext=/mfp/
languagePreferences=en

react-native run-android
