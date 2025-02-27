# zoo-argo-wf-proc-service-template
This repository serves as a template for creating processing services that utilize Argo Workflows within a ZOO Project environment.

## Features

- **Argo Workflows Integration**: Leverage Argo Workflows to define and manage workflows in Kubernetes.
- **ZOO Project Compatibility**: Designed to work seamlessly with the ZOO Project,.
- **Customizable Templates**: Easily adapt the template to fit specific processing service requirements.

## Getting Started

### Prerequisites

Before running the example, ensure the following are in place:

1. **Argo Workflows Deployment**: Deploy Argo Workflows using tools such as the [dev-platform-argo-workflows repository](https://github.com/fabricebrito/dev-platform-argo-workflows).  
2. **Workflow Template**: Deploy the [ZOO Argo Workflow Template](https://github.com/EOEPCA/zoo-argo-wf-workflow-template).

### Setup and Test

Follow these steps to clone, set up, and test the template:

1. **Clone the Repository**:  
    Clone the repository to your local environment:  
    ```bash
    git clone https://github.com/lmizzoni/zoo-argo-wf-proc-service-template.git
    cd zoo-argo-wf-proc-service-template
    ```
2. **Create and Activate a Python Virtual Environment**:
    Set up a Python environment to isolate dependencies:
    ```bash
    python -m venv env_zoo
    source env_zoo/bin/activate
    ```
3. **Install Dependencies**:
    Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    pip install -i https://test.pypi.org/simple/ zoo-argowf-runner  # (Pending release to PyPI)
    ```
4. **Run the Tests**:
    Use `nose2` to execute the tests and verify the setup:
    ```bash
    nose2
    ```