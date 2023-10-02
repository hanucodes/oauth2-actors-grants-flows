# oauth2-actors-grants-flows
OAuth 2.0 Tutorial and CheatSheat having OAuth Actors, Grant Types, Flows and OAuth Endpoints

# What is OAuth 2?

Suppose you want to use a great new third party application for Emails that has many awesome features you want. However, this new email application will need access to your Gmail emails in order to work.

Would you give you Gmail password to this third-party application? No.

So, how can this third-party app access our Gmail emails without getting your password?

OAuth 2.0 is one way.

Instead of providing your credentials to this third-party app, you will be redirected to Google OAuth Server. This OAuth Server will accept your Gmail credentials and provide a temporary Access Token to the Third-party app.

Now the third-party app can use this Access Token and access only your Gmail emails. The app cannot use this token to access any other data like your Google Drive. Also this Access Token has a validity after which the token will expire and will have to be re-generated.
