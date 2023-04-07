# magicAuth0
Quick demo how to connect Magic.io to a third-party IMS.

## Description
Magic.io's Wallet Services feature uses the OISC Oauth extension to facilitate the connection to a third-party IMS. In this example I am using Auth0 as the IDM and have built a simple single page application. The user authenticates using Auth0 and is issued a JWT. Then using the JWT and a providerId from Magic.io the user is authenticated to Magic.io. This provides a seemless integration between a companies authentication and Magic.io. Simplifies the user experience by providing all of the benefits of single sign on.

### Dependencies

* Auth0 SPA SDK
* Magic SDK
* Magic OIDC

Note: I am using CDNs

### Installing and Executing 

* Download or clone the repo
```
npm install && npm start
````
### Results

* Access Token Displayed
* auth.magic.link cookies

### Security

*  JWTs can use a public/private key pair in the form of an X.509 certificate for signing. A JWT can also be symmetrically signed by a shared secret using the HMAC algorithm. https://auth0.com/docs/secure/tokens/json-web-tokens#security