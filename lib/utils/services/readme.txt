We will be creating a different kind of service files in the folder lib/utils/services
Note: All the services will be singleton classes.
1) local_storage_service.dart: In this file, we write all the code needed to store and get data from the local storage using the plugin shared_preferences.
In this file, there will be getters and setters for each and every data to be stored in the local storage.
2) secure_storage_service.dart: We do not store user credentials, API tokens, secret API keys in local storage, for that we make use of flutter_secure_storage which stores data in the Android Keystore and Apple keychain with platform-specific encryption technique.
In this file, there will be getters and setters for each and every data to be stored in platform secure storage.
3) rest_api_service.dart: We do call the rest API to get, store data on a remote database for that we need to write the rest API call at a single place and need to return the data if the rest call is a success or need to return custom error exception on the basis of 4xx, 5xx status code. We can make use of http package to make the rest API call in the flutter
4) native_api_service.dart: We use multiple packages to access the native services like Camera, Photo Gallery, Location, etc for that we need to write code in a separate file which we can be used from multiple places throughout the application