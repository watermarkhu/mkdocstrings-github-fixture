# mkdocstrings-github-fixture

Fixture repository for testing [mkdocstrings-github](https://github.com/watermarkhu/mkdocstrings-github). 

## Repository Structure

This repository contains a comprehensive set of GitHub Actions and workflows designed to test the documentation generation capabilities of the mkdocstrings-github module.

### GitHub Actions

#### Root Level Actions
- **`action.yaml`** - Comprehensive root-level action with multiple input types, outputs, and branding

#### Actions in Subdirectories
- **`actions/simple-action/action.yml`** - Simple action with minimal configuration
- **`actions/complex-action/action.yaml`** - Complex action with advanced features, choice inputs, and comprehensive documentation
- **`actions/docker-action/action.yaml`** - Docker-based action demonstrating container execution
- **`actions/javascript-action/action.yml`** - JavaScript/Node.js-based action with pre/post hooks
- **`actions/minimal-action/action.yaml`** - Minimal action with only required fields
- **`actions/deprecated-action/action.yml`** - Action with deprecated features and edge cases
- **`nested/actions/deep-action/action.yml`** - Deeply nested action for testing directory discovery

### GitHub Workflows

#### Reusable Workflows (workflow_call)
- **`.github/workflows/reusable-workflow.yml`** - Comprehensive reusable workflow with inputs, secrets, outputs, and permissions

#### Manual Workflows (workflow_dispatch)
- **`.github/workflows/manual-dispatch.yml`** - Manual dispatch workflow with various input types and conditional logic

#### Hybrid Workflows
- **`.github/workflows/hybrid-workflow.yml`** - Workflow supporting both workflow_call and workflow_dispatch triggers
- **`.github/workflows/caller-workflow.yml`** - Workflow that calls the reusable workflow to demonstrate usage
- **`.github/workflows/complex-workflow.yml`** - Advanced workflow with matrix strategies, conditional jobs, and environment deployments

## Features Covered

### GitHub Actions Features
- ✅ Multiple input types (string, number, boolean, choice)
- ✅ Required and optional inputs with default values
- ✅ Multiline descriptions
- ✅ Output definitions with descriptions
- ✅ Branding (icon and color)
- ✅ Author information
- ✅ Different execution types (composite, docker, node)
- ✅ Actions at various directory levels
- ✅ Edge cases and deprecated features

### Workflow Features
- ✅ `workflow_call` trigger with inputs, secrets, and outputs
- ✅ `workflow_dispatch` trigger with various input types
- ✅ Hybrid workflows supporting multiple triggers
- ✅ Comprehensive permissions configurations
- ✅ Environment variables (global and job-level)
- ✅ Matrix strategies with includes and excludes
- ✅ Conditional job execution
- ✅ Job dependencies and outputs
- ✅ Environment deployments
- ✅ Parallel job execution
- ✅ Usage of local actions within workflows

### Input Types Demonstrated
- String inputs with defaults
- Number inputs with validation
- Boolean inputs
- Choice inputs with predefined options
- Multiline text inputs
- JSON configuration inputs

### Advanced Features
- Complex job orchestration
- Matrix builds with experimental configurations
- Environment-specific deployments
- Comprehensive error handling
- Workflow summaries and reporting
- Integration between workflows and local actions

## Testing the Documentation Module

This fixture repository provides comprehensive test cases for the mkdocstrings-github module to validate:

1. **Action Discovery**: Actions placed at various locations (root, subdirectories, nested paths)
2. **Workflow Discovery**: Workflows with different trigger types
3. **Metadata Extraction**: Complete extraction of descriptions, inputs, outputs, secrets, permissions
4. **Edge Case Handling**: Minimal configurations, deprecated features, missing descriptions
5. **Complex Scenarios**: Matrix strategies, conditional execution, hybrid triggers
6. **Integration Testing**: Workflows using local actions, reusable workflow patterns

## Usage

This repository serves as a test fixture and should not be used for actual CI/CD purposes. All actions and workflows are designed for testing documentation generation capabilities.
