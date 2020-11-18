# Command API Tutorial

This project is an exercise based on a Les Jackson's book:
*The Complete ASP.NET CORE API Tutorial.*

## Core concepts

### Basics

We're presented with a simple challenge, there's a plethora of CLI commands that we as developers must remember. This proves particularly difficult when we're jumping between languages and tools. This API fetches us a list of commands and their brief description.

For example:

![alt text](https://github.com/Piterino/commapitut/blob/main/exampleCommApiResult.png?raw=true)

### CI/CD Pipeline on Azure DevOps

The project uses continuous integration / continuous deployment - for new features to be implemented, only if they pass prior tests. In this case, our pipeline automatically recompiles and rehosts the service whenever we commit to master branch of our git repository.

### TDD

With a whole test suite unredlying all future work, TDD and CI/CD work in tandem to ensure high quality code.

### Switching environments and Data providers

In development we use a local docker postgres database, while in production we're using an Azure Linux container instance of postgres.

### Tokenization with Azure Active Directory

Our demon client app acquires a valid token from Azure Active Directory and becomes authorized to consume our API. By using a major trusted vendor, we delegate the responsibility and trust of issuing valid tokens outward.

### Environment variables and user secrets

Both in the local development environment and on Azure, we make use of key-value pairs stored as secrets to maintain confidentiality and keep our production endpoints secured.

### Unfortunately

**Due to my Azure free trial having expired and the charges incurred afterwards being higher than expected, the service is currently down.**
