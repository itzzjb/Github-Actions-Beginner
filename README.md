# I'm a Github Actions Beginner

**Here we are only trying to execute Testing on an event. Deploying and Building is not done here for now.**

Github Actions allows us to run an action whenever some event occurs on our repository.

**Events:**

- Pushing some code to a branch
- Creating a Pull request

**Actions:**

- Testing your code
- Deploying your code
- Building your code
- Run automatic scripts that can do activities like compiling files, moving code around, cleaning up the code base, closing an issue etc.

For more information we can refer to [Github Actions Website](https://github.com/features/actions).

> [!IMPORTANT]
> We can run any workflow in on any github event.

**Benefits:**

- We can use runners that are hosted for major operating systems to build and test projects.

  - Runners are hosted in VM or a container.
  - Github will automatically spin up runners for us. (Free up to a certain amount of minutes per month).
  - We can also use your own servers in cloud or on-prem to host runners too.

- We can have matrix workflows to simultaneously test across multiple operating systems and versions of your runtime.

- We can build, test, and deploy applications in a language of choice because github actions supports any language.

> [!NOTE]
> Mainly github actions is used every day to automatically the do the testing and making sure we don't put code that are potentially broken or doesn't pass any test to a main branch or production branch.

**Created a basic flask application and unit tests for it.**

## What we expect here ?

Whenever we change something in the repository, we want to automatically run our test.

We need to write scripts to run all the test and check whether they are passed before we give someone the ability to merge the code.

## Branch Protection Rules

By adding this, we can make the repository as no one is able to push directly to main or master branch. Instead they have to create a pull request if they want to contribute.

Main / Master branch should be always clean and fully functioning. So, you don't want to accidentally push something to the main branch when working with multiple people.

We need to ensure that it pass all the different tests and the pull request should be approved in order to merge into the main / master branch.

> [!IMPORTANT]
> Make sure to

## Setting up a github workflow

1. We need to create a `.github` directory in the root folder.
2. Inside it we can create a directory called `workflows`. (We have other types of actions like deployment that can be added here too)
3. We put all the syntax, triggers, scripts we want to run inside a `.yml` file. (Give a meaningful name for the workflow)

## Defining the workflow

You can find github workflow triggers [Here](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows).

You can visit the [Github Marketplace](https://github.com/marketplace) to find pre-written scripts and more.
