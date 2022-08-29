# Introduction

Terrakube is an open source collaboration platform for running remote infrastructure as code operations using terraform that aims to be a complete replacement for close source tools like Terraform Enterprise, Scalr or Env0.

The platform can be easily installed in any kubernetes cluster, you can easily customize the platform using other open source tools already available for terraform (Example: terratag, infracost, terrascan, etc) and you can integrate the tool with different authentication providers like Azure Active Directoy, Google Cloud Identity, Github, Gitlab or any other provider supported by [Dex](https://dexidp.io/docs/connectors/).

Terrakube provides different features like the following:

* Terraform module protocol:
  * This allows Terrakube to expose an open source terraform registry that is protected and is private by default using different Dex [connectors](https://dexidp.io/docs/connectors/) for the authentication with different providers.
* Terraform provider protocol:
  * This allows Terrakube to expose an open source terraform registry where you can have create your own private terraform providers or create a mirror of the current terraform providers available in the public Hashicorp registry.
* Handle you infrastructure as code using Organization like closed source tools like Terraform Enterprise and Scalr.
* Easily extended by default integrating with many open source tools available today for terraform CLI.
* Support to run the platform using any **RDBMS** supported by [liquibase](https://www.liquibase.org) (mysql, postgres, oracle, sql server, etc).
* Plugins support to extends functionality using different cloud providers and open source tools using the Terrakube Configuration Languague (TCL).
* Easily extends the platform using common technologies like react js, java, spring, elide, liquibase, groovy, bash, go.
* Native integration with the most popular VCS like:
  * Github.
  * Azure DevOps
  * Bitbucket
  * Gitlab
* Support for SSH key (RSA and ED25519)
* Handle Personal Access Token
* Extends and create custom flows when running terraform remote operations with custom logics like:
  * Approvals
  * Budget reviews
  * Security reviews
  * Custom logic that you can build with groovy and bash scripts
