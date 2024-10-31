# GitHub User and Repository Data (Delhi:100)

- Data scraping was done using the GitHub REST API to fetch user and repository details in Delhi with over 100 followers.
- It was surprising to find that a significant portion of repositories in Delhi have no licenses, potentially limiting reuse.
- Recommendation: Developers should prioritize licensing their projects to encourage sharing, use, and collaboration within the GitHub community.

## Project Overview

This project contains two main datasets:

1. **users.csv** - Details of GitHub users from Delhi with over 100 followers.
2. **repositories.csv** - Public repository data for these users, with up to 500 of their most recently pushed repositories.

## Data Collection Process

Using the GitHub REST API, we retrieved and filtered user and repository data:
- `users.csv` captures essential user details including bio, company, location, and follower count.
- `repositories.csv` includes repository metadata, such as creation date, language, and star count.

## Data Cleaning

Data fields were cleaned as follows:
- `company` names were standardized by trimming whitespace, removing leading `@` symbols, and converting to uppercase.
- Null values were replaced with empty strings.
- Boolean values were normalized as `true` and `false`.

## Key Insights

After analyzing the data, we observed:
- A majority of the repositories do not have licenses, which may discourage open-source contributions.
- Certain languages, such as Python and JavaScript, are predominant among developers in Delhi, reflecting current industry trends.

## Recommendation

Encouraging developers to license their repositories can significantly enhance code sharing and community collaboration.
