https://duckster.medium.com/the-truth-about-api-management-in-a-microservice-architecture-a3b001a713c5

## User impersonation

https://www.youtube.com/watch?v=ACZQk61Iq9I

## Secure ASPNet Web API

For example, in an ASP.NET Core Web API that exposes RESTful endpoints that might be accessed by
Single Page Applications (SPAs), by native clients, or even by other Web APIs, you typically want to
use bearer token authentication instead. These types of applications do not work with cookies, but
can easily retrieve a bearer token and include it in the authorization header of subsequent requests.

## Keycloak federation Active Directory

https://medium.com/@yasithkumara/active-directory-as-a-user-federation-in-keycloak-926fd7cc3256

## Kerberos KeyCloak SSO

https://www.keycloak.org/docs/latest/server_admin/index.html#_kerberos

## Keycloak SSO with React

https://medium.com/@gmonne/keycloak-sso-1813a2072d64

## Securing with KeyCloak

### Part One: Installing Keycloak with Docker and Administration

https://medium.com/p/1d076777a979

### Part Two: Securing a front-end React application

https://blog.devgenius.io/security-in-react-and-webapi-in-asp-net-core-c-with-authentification-and-authorization-by-keycloak-89ba14be7e5a

https://blog.devgenius.io/security-in-react-and-webapi-in-asp-net-core-c-with-authentification-and-authorization-by-keycloak-f890d340d093

```bash
curl \
  -d "client_id=MyApp" \
  -d "username=galamome" \
  -d "password=galamome" \
  -d "grant_type=password" \
  "http://localhost:8081/realms/MyRealm/protocol/openid-connect/token"
