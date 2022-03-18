# camunda-spring

Camunda Platform is an open-source workflow and decision automation platform. Camunda Platform ships with tools for creating workflow and decision models, operating deployed models in production, and allowing users to execute workflow tasks assigned to them.

Adding automation to our application should not be authorized for public. Only specific users (mods), are allowed to deploy models so others could only use them, prohibiting others to create arbitrary workflows.

Our application will probably have a modern microservice architechture so we could consider this code as a submodule of a huge appplication running on top of Spring Boot (Java based framework).

Creating a Single Sign-On (SSO) is an authentication scheme is highly encouraged so we implemented a Keycloak realme that contains all the settings needed for our application to run properly.

We used a special camunda plugin called ```camunda-bpm-identity-keycloak``` for this purpose. I will provide everything in the ```references```  section so you could deep dive into the implementation.

# references
* https://github.com/camunda-community-hub/camunda-bpm-identity-keycloak
