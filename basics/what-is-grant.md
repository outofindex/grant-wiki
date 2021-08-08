
Having to login your users to your app is a necessity. However, it is considered a bad practice to handle the user's login credentials, such as user name and password yourself. In general having a login form on your website and subsequently storing the user credentials in your own database is a security concern.

For that reason people invented OAuth, a framework to delegate the login form and credentials to a trusted third-party provider, for example Google or Twitter. This covers the Authentication part.

Outside of that OAuth can also be used for Authorization - granting access to for your OAuth app to the user's owned resources on a third-party platform.

Grant is a tool to help you login using OAuth to any third-party provider, and receive back the credentials needed to access that provider. With just a little bit of static JSON configuration you can instantiate Grant on any of the most popular HTTP server frameworks for Node.js, and on any of the most popular Serverless Cloud Providers.
