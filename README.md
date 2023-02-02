# Backend Engineer Coding Challenge

> This repository contains the coding challenge for backend engineers.

**Note:** Please don't fork this repository, create a pull request against it, or use GuardRails in the repo name. Otherwise other candidates may take inspiration from it. Once the coding challenge is completed, please sumbit your test on Greenhouse.

## Description

Build a simple code scanning application that detects sensitive keywords in public git repos.
The application must fulfil the following requirements:
- A user can CRUD repositories. A repository contains a name and a link to the repo
- A user can trigger a scan against a repository
- A user can view the Security Scan Result ("Result") List

How to do a scan:
- Just keep it simple by iterating the words on the codebase to detect secrets findings
- A secret starts with the prefix `public_key` or `private_key`

The Result entity should have the following properties and be stored in a database of your choice:
- a unique id
- the scan's status (one of "Queued" | "In Progress" | "Success" | "Failure")
- the repsository name
- the repsository URL
- the findings, see [example](example-findings.json) for an example
- timestamps that indicate when a scan was enqueued, as well as when the scan started and finished

**What we want to see:**
- Project Structure: Clear organization and structure of folders, code and functionality
- Idiomatic Code: Following established community standards, code consistency, use of linters, formatting, error handling, and anything else that shows your skills. Simple is better than complex
- Stack Knowledge: Proper use of Golang and selected frameworks / libraries
- Implementation: The implementation has to work according to the specs
- Unit Tests: Covering the core functionality with unit tests
- Proper Documentation: 
    - A High-Level Design for the components / infrastructure if any
    - Describe how you came up with the solution and what makes it a good one for the use-case
    - Describe how to configure the project, how to start it, how to test it etc
- SQL schema: proper modeling all entities and their relationship on the DB level

**Bonus points for:**

- API documentation
- Use of appropriate design patterns
- Code comments

**Things you don't have to worry about:**

- Authentication / Authorization
- CI configuration / Deployment
- APM


## Scoring

| General                | Points |
|------------------------|--------|
| Project structure      | 0-3    |
| Idiomatic code         | 0-3    |
| Stack Knowledge        | 0-3    |
| Implementation         | 0-3    |
| Unit tests             | 0-3    |
| README & Documentation | 0-3    |
| Commit messages        | 0/1    |
| Libraries              | 0/1    |
| SQL Schema             | 0/1    |

| Bonus             | Points |
|-------------------|--------|
| Code Comments     | 0/1    |
| API Documentation | 0/1    |
| Design Patterns   | 0/1    |
| Architecture      | 0/1    |

Maxium points: 25
