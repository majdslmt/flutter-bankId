# flutter-bankId

### This is an example of how to connect a Flutter app with OAuth2 BankID using Identity Server as the backend or Identity Provider (IDP). 

You need to add appAuthRedirectScheme to android app 

Add appAuthRedirectScheme to build.gradle 
```
manifestPlaceholders += [
                'appAuthRedirectScheme': 'bankiddemo'
        ]
        
```
Add also to AndroidManifest.xml
```
<data android:scheme="${appAuthRedirectScheme}"/> <!-- reference the placeholder here -->
```
