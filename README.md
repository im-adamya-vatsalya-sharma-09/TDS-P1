# GitHub Users and Repositories Analysis

- I used the GitHub API to find users in Basel with over 10 followers. For each user, I fetched their details and up to 100 recent repositories, compiling the results into users.csv and repositories.csv while cleaning and formatting the data accordingly.

## Project Overview
This project aims to analyze GitHub users based in Basel who have more than 10 followers. By leveraging the GitHub API, we gather user information and their public repositories to uncover insights into user engagement, repository activity, and the impact of licensing on repository visibility.

## Data Collection Methodology
- **API Utilization**: The GitHub API was employed to identify users in Basel with over 10 followers. The data collection process involved the following steps:

- **User Information**: For each user, the retrieved essential details includes:
        
      login: GitHub user ID
      name: Full name of the user
      company: The user's company (cleaned and formatted)
      location: User's city
      email: User's email address
      hireable: Whether the user is open to job opportunities
      bio: A short bio provided by the user
      public_repos: Number of public repositories
      followers: Number of followers
      following: Number of users they are following
      created_at: Account creation date
- **Repository Data**: For each user, up to 100 recent repositories were fetched, capturing the following details:

      login: GitHub user ID of the owner
      full_name: Full name of the repository
      created_at: Creation date of the repository
      stargazers_count: Number of stars received
      watchers_count: Number of watchers
      language: Primary programming language used in the repository
      has_projects: Whether the repository has projects enabled
      has_wiki: Whether the repository has a wiki
      license_name: Name of the license under which the repository is categorized

## Data Cleaning and Formatting 
The collected data was meticulously cleaned and formatted:

- Trimming whitespace from company names
- Stripping leading @ symbols from company names
- Converting company names to uppercase for consistency
- Representing boolean values as true, false, or empty strings for null values
## Output Files
The final processed data was compiled into two CSV files:

- users.csv: Contains detailed information about users.
- repositories.csv: Contains details about each user's public repositories.
- gitscrap.py: This Python script extracts GitHub user data from Basel with over 10 followers using the GitHub API. It fetches user details, repositories, and saves them into CSV files. The code manages API requests with a GitHub token, filters company names, and structures data for easy analysis.

## Conclusion
The analysis underscores the importance of user engagement and the potential positive effects of licensing on repository visibility. Through the effective use of the GitHub API, this project provides valuable insights that can guide developers in enhancing their presence and impact on the platform.

## Future Work
- **Explore Additional Factors:** Future analyses could delve into other aspects influencing user engagement, such as the frequency of repository updates, detailed documentation, and user interaction patterns.
- **Broader Scope:** Expanding the study to include users from different cities or regions may yield insights into varying engagement trends across geographic locations.
- **Community Feedback:** Gathering feedback from the GitHub community regarding their experiences with licensed repositories could provide qualitative insights that complement the quantitative findings.

## Acknowledgments
Special thanks to GitHub for providing a comprehensive API that allows developers to access valuable user and repository data, enabling insightful analyses and contributions to the open-source community.

