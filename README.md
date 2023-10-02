# oauth2-actors-grants-flows
OAuth 2.0 Tutorial and CheatSheat having OAuth Actors, Grant Types, Flows and OAuth Endpoints

# What is OAuth 2?

https://helpercodes.com/oauth-2-0-tutorial-what-is-oauth-2/

Suppose you want to use a great new third party application for Emails that has many awesome features you want. However, this new email application will need access to your Gmail emails in order to work.

Would you give you Gmail password to this third-party application? No.

So, how can this third-party app access our Gmail emails without getting your password?

OAuth 2.0 is one way.

Instead of providing your credentials to this third-party app, you will be redirected to Google OAuth Server. This OAuth Server will accept your Gmail credentials and provide a temporary Access Token to the Third-party app.

Now the third-party app can use this Access Token and access only your Gmail emails. The app cannot use this token to access any other data like your Google Drive. Also this Access Token has a validity after which the token will expire and will have to be re-generated.

# OAuth 2.0 Tutorial: Part 1 OAuth Actors

[OAuth Actors and their Role Table View](https://helpercodes.com/oauth-2-0-tutorial-part-1-oauth-actors/)

Resource Owner	
1. owns resources – like email
2. owns login credentials
3. delegates access to Third-party application

Client
(Third-party application)	
1. wants to get access to resources to provide some functionality
2. holds access tokens
3. ideally should not hold password of resource owner
4. identified via ClientI D and Client Secret

OAuth Servers	
1. Login Page component
2. LDAP Server to validate user password
3. Consent Page component
4. Token Database component
5. Exposes 2 enpoints

Resource Server	
1. Holds Resources
2. Protects Resources – via direct password by user
3. Protects Resources – via OAuth Access Tokens by Third Party Apps

