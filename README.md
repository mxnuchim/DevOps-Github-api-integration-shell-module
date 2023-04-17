# Shell Script Module for GitHub API

This shell script module allows users to retrieve information from GitHub by talking to its API. It can also be modified to work with other applications like JIRA, GitLab, and others.

## Prerequisites

In order to use this script, you will need to have the following installed:

- [cURL](https://curl.se/)
- [jq](https://stedolan.github.io/jq/)

## Getting Started

1. Create a file in your terminal and paste script into it

```
vim github.sh
```

2. Make the script executable.

```
chmod +x github.sh
```


3. Execute the script with the appropriate arguments.

```
./github.sh <PERSONAL_ACCESS_TOKEN> /orgs/<YOUR_ORGANIZATION>/repos
```

Note: Replace `<PERSONAL_ACCESS_TOKEN>` with your own GitHub personal access token, and `<YOUR_ORGANIZATION>` with your own GitHub organization name.

## Usage

This script takes two arguments:

1. `<PERSONAL_ACCESS_TOKEN>` - Your GitHub personal access token. This is required to authenticate your request to the GitHub API.

2. `/orgs/<YOUR_ORGANIZATION>/repos` - The URL path to the API endpoint you wish to retrieve data from. This can be modified to work with any other applications like JIRA, GitLab, and others.

## Example

Here is an example command to call the script:

```
./github.sh abcdefghijklmnopqrstuvwxyz0123456789abcdef /orgs/acme-corp/repos
```
To return information about all repositories in your organization


Or

```
./github.sh abcdefghijklmnopqrstuvwxyz0123456789abcdef /user
```
To return information about you (User)

## Contributing

If you'd like to contribute to this project, please feel free to submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
