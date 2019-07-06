# Passport SAML WSO2

A simple express application with passport-saml configurations for WSO2 SAML2 SSO.

## Install

Execute the following command from the root folder to install all necessary dependencies

```shell
npm install
```

## Configure

### Express Application

Create a `.env` file in the root directory and enter the following properties

> Change the `SAML_ENTRYPOINT` and `SAML_LOGOUTURL` if the ip-address and ports are different from default configurations

```env
SESSION_SECRET="a well secured secret"

SAML_ENTRYPOINT="https://localhost:9443/samlsso"
SAML_ISSUER="SampleExpressApp"
SAML_PROTOCOL="http://"
SAML_LOGOUTURL="https://localhost:9443/samlsso"

WSO2_ROLE_CLAIM="http://wso2.org/claims/role"
WSO2_EMAIL_CLAIM="http://wso2.org/claims/emailaddress"
```

## Run

Use the following command to start the express application

```shell
npm start
```

or

```shell
nodemon server.js
```

navigate to [http://localhost:3000/app](http://localhost:3000/app)
