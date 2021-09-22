# cap-server-url

### how to wrap a Next.js application to capacitor using server.url

- create a empty folder and run `npm init -y`
- install capacitor dependencies `npm install @capacitor/core
npm install @capacitor/cli --save-devn npm install @capacitor/android`
- Then, initialize Capacitor using cli run `npx cap init` 
- Then add this `"server": {
		"url": "https://confident-kilby-f04655.netlify.app/"
	}` in capacitor.config.json
  - Add the Android Platform to your project run `npx cap add android`
  - Create a assets folder in side `android\app\src\main\assets` and create two files `capacitor.config.json` and `capacitor.pugins.json`
  -  Run `npx cap sync` it will copy web assets and plugins to android
  -  Then run `npx cap run android` to run on your phone
