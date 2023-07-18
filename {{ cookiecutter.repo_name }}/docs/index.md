# {{ cookiecutter.project_name }}

> **Everything in comment blocks are placeholder text that you should replace with actual, project-specific descriptions.**

> **Code version (Git commit hash):** {YOUR_CODE_COMMIT_HASH}

## Overview

{{ cookiecutter.description }}

### Background

> Briefly introduce the background and motivation of this project. Show the reason why this project exists and is needed in a few words.

### Target

> The aim of the project. What output can we consider this project to be successful.

### Dependencies

> Necessary conda environment, Docker image, or software to run this project.

- [Conda environment](../environment.yaml)

### Resource Requirements

> List CPU, GPU, memory, and IO requirements for executing the workflow for typical use case.

## Inputs and Parameters

### Input Data

> 1. **{YOUR_DATASET_NAME} (should be a project name if using internal data)**
>
>    - **Description**: Briefly describe details of the datasets
>    - **Data type**:
>    - **Dataset size**:
>    - **Path**:
>    - **Processing procedure**: Clearly document any data preprocessing steps performed on the raw data, such as cleaning, filtering, or aggregating, along with the rationale behind each step. If EDA needs to be done to the data, it may need another document/project to show the details.
>
> 2. ...

### Key Parameters

> 1. **{YOUR_PARAMETER_NAME}**
>
>    - **Description**: Briefly describe the meaning of the parameter and how to set it properly.
>    - **Value**: The value of the parameter used in the project.
>
> 2. ...

## Workflow Steps

> Describe each step of the workflow in a sequential manner, and provide a flowchat to describe the relationship between each module in the pipeline.
>
> Include details such as the specific algorithms or methods used, software libraries, and versions.
>
> Provide clear instructions on how to execute each step, including any necessary command-line arguments or configuration files.

## Results and Outputs

> Document the expected results and outputs of the workflow. Include any generated files, reports, visualizations, or metrics. Specify the format and structure of each output.
>
> - **{YOUR_OUTPUT_NAME}**: {YOUR_OUTPUT_PATH}

## Conclusion

> The conclusion of this document.
