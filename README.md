
# Library Management System

This is a Library Management System (LMS) app that helps manage library members, articles, and transactions. It allows you to issue and return articles, track membership validity, and more.

## Table of Contents
- Features
- Installation
- Usage
- License

## Features
### Library Member Management:

- Add and update members with their first name, last name, and full name.
- Membership is validated before issuing articles.

### Library Membership:

- Members can have a valid membership with start and end dates.
- Membership automatically expires after a set period.
- Prevents members from having overlapping active memberships.

### Articles:

- Add articles (books, journals, etc.) to the system.
- Track article status (Available or Issued).
- Display details like title, author, publisher, ISBN, and description.

### Library Transactions:

- Issue and return articles.
- Track article status changes to "Issued" or "Available".
- Ensure that members cannot exceed the maximum number of articles issued.

## Installation
1. Clone the repository:

```bash

git clone https://github.com/your-username/your-repository-name.git
```
2. Navigate to the app directory:

```bash

cd your-repository-name
```
3. Install dependencies:

- Make sure you have frappe installed in your environment.
- Run the following command to install any additional dependencies.
```bash

pip install -r requirements.txt
```
4. Setup the app:

- Use Frappe commands to install the app in your bench.
```bash

bench new-site your-site-name
bench --site your-site-name install-app library_management_system
```

## Usage

### Add a Library Member:
- Go to the "Library Member" section and add a new member.
  
### Create a Library Membership:
- Create a new membership for the member, set the start date, and the system will automatically calculate the end date.
  
### Issue Articles:
- Select an article, issue it to a member, and check its status (it will change to "Issued").

### Return Articles:
- When a member returns an article, its status changes back to "Available".

## License
- This project is licensed under the MIT License - see the LICENSE file for details.

