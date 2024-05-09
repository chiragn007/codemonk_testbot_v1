# Codebase Repository

Welcome to the `codebase` repository! This repository primarily focuses on refactoring code and implementing user requests. If you're here, it means you're interested in understanding or contributing to the project. This README will guide you through the basics.

## Overview

The `codebase` repository is designed to streamline the process of code refactoring and user request implementation. Whenever an issue is raised on GitHub, the Continuous Integration (CI) system is triggered via webhooks. The CI system then identifies the necessary changes required to resolve the issue, modifies the relevant files, and finally creates a pull request with the modifications.

## How It Works

1. **Issue Raised**: A user or team member raises an issue on the GitHub repository, specifying the problem or feature request.

2. **Webhook Trigger**: GitHub's webhook system detects the new issue and sends a notification to the Continuous Integration (CI) system.

3. **Automated Refactoring**: The CI system analyzes the issue, identifies the code sections that need modification, and applies the necessary changes to the codebase.

4. **Pull Request Creation**: After the modifications are made, the CI system automatically creates a pull request on GitHub, allowing the changes to be reviewed and merged.


## Running the Code

To run the `codebase` project locally, follow these steps:

1. **Clone the Repository**:

    ```
     git clone https://github.com/chiragn007/codebase.git
    ```

3. **Install Dependencies**: Navigate to the root directory of the cloned repository and run:

    ```
      pip install -r requirements.txt
    ```


4. **Set Environment Variables**: 
- Set the GPT API key:
  ```
  export GPT_API_KEY=your_gpt_api_key_here
  ```
- Set the GitHub token access:
  ```
  export GITHUB_TOKEN=your_github_token_here
  ```

4. **Run the Application**: From the root directory, execute the following command:

   ```
     uvicorn main:app --reload
   ```

After running the application, you can view the API documentation at [http://127.0.0.1:8000/api/v1/docs](http://127.0.0.1:8000/api/v1/docs).
