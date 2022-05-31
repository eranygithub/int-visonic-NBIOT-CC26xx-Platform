# Repository Contribution Standards

## Description
This repository contains all the relevant code for the <NBIOT-CC26xx-Platform>

# Support
[Fusion DevOps team](https://github.com/orgs/jci-products/teams/fusion/members)
# jci-github-repository-template
Template repository from which to create all others
  
# More information
Reference the [JCI GitHub Information Sharepoint](https://my.jci.com/sites/GitHub) for all things GitHub, especially the [Source Control Standards](https://my.jci.com/:b:/r/sites/GitHub/Shared%20Documents/Source+Control+Standards+v1.0.2.pdf?csf=1&web=1&e=hTT37y) that define the content of this template

# Rules Enforced
This template repository comes with a `main` branch protection rule configured that implements the requirements of standards GH.M.02 and GH.M.03

# Content Provided
This repository contains a `README` file that you can use as a guide or template for your own `README.md` that implements the guidelines in GH.O.05


## Branching Strategy

##################### <$MAKE-SURE-TO-SELECT-ONLY-ONE-SET$> ##############################################
############## <$SINGLE-PROJECT-REPO-WORKING-BRANCHES$> ##############
This repository allows for the following working branches:
- feature/\<JIRA-ticket>
- bugfix/\<short-description> or \<JIRA-ticket>

This repository supports the following permanent branches:
- main
- master
- release/\<release-version>

<details>
  <summary>Branch Naming Regex (Click to Expand)</summary>

    ^(feature/[A-Z0-9]{2,6}-[0-9]{1,8}([-_]{1}[-_a-zA-Z0-9]*)*)$
    ^(bugfix/[-_a-zA-Z0-9]*)$
</details>

<details>
  <summary>Branch Naming Examples (Click to Expand)</summary>

    feature/ABC-1234
    feature/ABC-1234_text_text
    bugfix/ABC-1234_text_text
    bugfix/text_text
    release/4.2.0
</details>

############## <$MULTI-PROJECT-REPO-WORKING-BRANCHES$> ##############
This repository allows for the following working branches:
- \<project-prefix>\/feature/\<JIRA-ticket>
- \<project-prefix>\/bugfix/\<short-description> or \<JIRA-ticket>

This repository supports the following permanent branches:
- master
- master_unstable
- \<project-prefix>/main
- \<project-prefix>/release/\<release-version>

<details>
  <summary>Branch Naming Regex (Click to Expand)</summary>

    ^([a-z0-9_]{2,15}/feature/[A-Z0-9]{2,6}-[0-9]{1,8}([-_]{1}[-_a-zA-Z0-9]*)*)$
    ^([a-z0-9_]{2,15}/bugfix/[-_a-zA-Z0-9]*)$
</details>

<details>
  <summary>Branch Naming Examples (Click to Expand)</summary>

    \<project-prefix>/feature/ABC-1234
    \<project-prefix>/feature/ABC-1234_text_text
    \<project-prefix>/bugfix/ABC-1234_text_text
    \<project-prefix>/bugfix/text_text
    \<project-prefix>/release/4.2.0
</details>

##########################################################################################################

---

## GpG
All commits must be signed with a GpG key, regardless of the branch. Pull requests from branches that have unsigned commits WILL be blocked.

---

## Pull Requests
Contributions to permanent branches is via pull requests from working branches only! 
A pull request linter is in effect.

### Pull Request Syntax
\<Prefix>\<Whitespace>\<Summary>
- \<Prefix> - is an indicator of the change; either \[JIRA_PREFIX-JIRA_TICKET_NUMBER] to denote the JIRA task or \[BF] to denote a bugfix
- \<Whitespace> - separator between the prefix and summary, MUST be ' ' (space)
- \<Summary> - a short summary of the contribution; CANNOT contain special characters!

<details>
  <summary>Valid Pull Request Titles (Click to Expand)</summary>

    [LCH-1234] This is a summary of the change
    [BF] Some description
</details>

<details>
  <summary>Invalid Pull Request Titles (Click to Expand)</summary>

    LCH-1234: This is a summary of the change
    some bug fix
</details>

---
 
# About the project:
## Project Name
<TBD> - populated by development team

## Owners / Maintainers
<TBD> - populated by development team

## Any extra fields can be added here
<TBD> - populated by development team
 
## Licensing
Internal JCI usage only

---
 

