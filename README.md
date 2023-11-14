The purpose of the provided shell script project is to interact with the GitHub API 
and retrieve information about users who have read access (pull permissions) to a specified GitHub repository. 
Here's a breakdown of the project's main components and purpose:

1. **GitHub API Integration:**
   - The script utilizes the GitHub API to fetch data. It constructs the API URL and uses the `curl` command to make HTTP requests.
   - The authentication is handled using a GitHub username and personal access token. This ensures that the script has the necessary
   - permissions to access the required data.

2. **Function to Make API Requests:**
   - The `github_api_get` function is responsible for making a GET request to the GitHub API. It takes an API endpoint as an argument
   - and constructs the full URL before making the request.

3. **Listing Users with Read Access:**
   - The main functionality of the script is to list users with read access to a specified GitHub repository (`list_users_with_read_access` function).
   - It queries the GitHub API for the list of collaborators on the specified repository and filters out users with pull (read) permissions.

4. **Main Script Execution:**
   - The main part of the script prompts the user for the repository owner and name, then calls the function to list users with read access to
   -  that repository.

5. **Output:**
   - The script outputs the list of users with read access to the specified repository. If no such users are found, it provides a corresponding message.

The overall purpose of the project is to automate the process of fetching and displaying information about users who have read access to a GitHub repository.
This can be useful for repository management, access control, or any scenario where knowing who has read permissions on a repository is necessary.

You can customize and extend this script based on your specific needs, adding more functionalities or error handling as required.
