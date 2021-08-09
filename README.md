
Having to login your users to your app is a necessity. However, it is considered a bad practice to handle the user's login credentials, such as user name and password yourself. In general having a login form on your website and subsequently storing the user credentials in your own database is a security concern.

For that reason people invented OAuth, a framework to delegate the login form and credentials to a trusted third-party provider, for example Google or Twitter. Besides Authentication, OAuth can also be used for Authorization - granting access to your OAuth app to access resources on behalf of the user.

[Grant] is a tool to help you login using OAuth to any third-party provider, and receive back the user's identity information and/or credentials needed for accessing that provider on behalf of the user.

With only a few lines of static JSON configuration you can instantiate Grant on any of the most popular HTTP server frameworks for Node.js, and on any of the most popular Serverless Cloud Providers.

Grant can be fully configured dynamically over HTTP, meaning that you can host it as a standalone service and integrate it with any other backend service or programming language.

  [grant]: https://github.com/simov/grant
