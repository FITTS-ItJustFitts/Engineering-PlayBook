The basics are:

- We have unit tests that each developer runs on their own machine.
- When they commit their code to git, the tests are run again, "integrated" with code from other developers.

This helps ensure there's nothing specific to the developer's machine making the tests pass.
The code in version control needs to run cleanly in production later so before the code is allowed to be deployed to production,
it is run on a CI server or service.

For continuous integration, we use [Azure Pipeline](https://azuredevopslabs.com/labs/azuredevops/continuousintegration/)

CI test runs are triggered when we push to Github and can be seen as part of the status checks of pull requests.
