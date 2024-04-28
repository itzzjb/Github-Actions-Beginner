# I'm a Github Actions Beginner

Github Actions allows us to run an action whenever some event occurs on ou repository.

**Events:**

- Pushing some code to a branch
- Creating a Pull request

**Actions:**

- Testing your code
- Deploying your code
- Building your code
- Run automatic scripts can do activities like compiling files, moving code around, cleaning up the code base, closing an issue etc.

For more information we can refer to [Github Actions Website](https://github.com/features/actions).

> [!IMPORTANT]
> We can run any workflow in on any github event.

**Benefits:**

- We can use runners that are hosted for major operating systems to build and test projects.

  - Runners are hosted in VM or a container.
  - Github will automatically spin up runners for us. (Free up to a certain amount of minutes per month).
  - You can also use your own servers in cloud or on-prem to host runners too.

- We can have matrix workflows to simultaneously test across multiple operating systems and versions of your runtime.

- We can build, test, and deploy applications in your language of choice because github actions supports any language.

> [!NOTE]
> Mainly github actions is used every day to automatically the testing and making sure we don't put code that are potentially broken and doesn't pass any test to the main branch or production branch.
