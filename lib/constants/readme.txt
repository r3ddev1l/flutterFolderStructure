1) api_path.dart: When using REST API service in dart then we can store all the API endpoints in a separate file api_path.dart

2) assest_path.dart: Although we have described the assets path in pubspec.yaml but to use that asset in an application we need to give there relative path in any widgets.
If we add all the assets relative path in one file then it will be easy for us to get all the paths and update the path if required in the future.

3) app_constants.dart: This is where all our application constants will be present and this is different for each application.