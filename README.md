# IT-Projekt
This project will not work alone because the Hashicorp Vault and the Keycloak Provider are not shipped with the project.

The project implemented a service based on gRPC which tokenizes values based on the FPE implementation by Bouncy Castle. 
A call to the service is authenticated by a Keycloak provider- to ensure an OAuth2 workflow. 
The generated dataset is stored securely inside a Hashicorp Vault. Additionally, the service uses mTLS to connect to 
the Keycloak and Hashicorp vault.

