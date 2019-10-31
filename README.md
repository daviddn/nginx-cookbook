# Chef

Chef is a configuration management tool of infrastructure. It will create environments with provision scripts, test code in the environments, and destroy the environments.

## Recipes

A recipe is a provisioning script - written in pure Ruby with its own methods (DSL - domain-specific language).

These live in the 'recipes' folder.

## Cookbooks

Holds many recipes.

## Test Kitchen

- Creates an environment for testing the Cookbook
- Runs the Chef code against the environment to provision it
- Runs unit tests (test the code) and integration test suites to ensure that the environment is correct/standardized (test the environment)
- Closes everything down

### Commands to use Chef and Kitchen

#### Create a VM

    $ kitchen create

#### Run recipes

    $ kitchen converge

#### Setup kitchen to run test

    $ kitchen setup

#### Run test on newly created environment

    $ kitchen verify

#### Destroy a VM

    $ kitchen destroy

#### Create, converge, setup, verify, and destroy

    $ kitchen test
