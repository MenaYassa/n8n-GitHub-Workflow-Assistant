GitHub Workflow Assistant

Author: Mena Yassa

This n8n-powered workflow acts as an intelligent assistant for managing GitHub repositories. It provides capabilities for repository structure exploration, file content analysis, and branch management, offering a streamlined approach to interacting with GitHub repositories.

Features

Automated repository structure analysis and navigation

File content retrieval

Branch listing and comparison

Secure GitHub API integration

Use Cases

Repository Exploration

Navigate through repository directories and files

Retrieve specific files or code snippets

Branch Management

List all branches in a repository

Compare branches to identify changes

Code Understanding

Analyze repository structures

Understand key files and project organization

How to Use

Trigger the workflow via the webhook endpoint provided by n8n.

Send a POST request with the desired query structure:

{
    "query": "Your action or question",
    "repository_url": "The GitHub repository URL",
    "additional_params": {
        "param_name": "param_value"
    }
}

Example actions supported by the workflow:

"Get the repository structure"

"List all branches"

"Compare two branches"

"Retrieve content of a specific file"

Example Queries

"What is the structure of this repository?"

"Show me the contents of README.md in the repository"

"List all branches in this repository"

"Compare the 'main' branch with 'development'"

Limitations

Requires valid GitHub repository URLs

Limited to accessible repositories as per API credentials

Response times depend on repository size and query complexity
