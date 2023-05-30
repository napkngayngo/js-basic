# DEVELOPMENT GUIDE

First time, you need to clone project

```bash
$ git clone <repo_url>
```

Then every time you write a new section you need to do the following steps:

1. Create new branch

- Checkout `main` branch

```bash
$ git checkout main
```

- Pull latest code

```bash
$ git pull
```

- Create new branch based on title of content

```bash
$ git checkout -b <branch_name> 
# eg: you might write content for `Variables` section, the branch name will be `docs/variables`
# git checkout -b docs/variables
```

2. Create markdown file

```bash
# you might write content for `Variables` section
$ touch docs/variables.md
```

3. Write content with Markdown

- Markdown basic syntax ([reference](https://www.markdownguide.org/basic-syntax/))
- Markdown extended syntax ([reference](https://www.markdownguide.org/extended-syntax/))

4. Link document content to table of contents

```markdown
## Table of contents

4. [Variables](docs/variables.md) <!-- link to file -->
    - [Variable declarations](docs/variables.md#variable-declarations) <!-- link to section with hash link -->
```

*Note: <b>Headings syntax</b> (https://www.markdownguide.org/basic-syntax/#headings) will be parsed to hash-link automatically,
eg: the "Variable Declarations" header in `docs/variables.md` is corresponding to `docs/variables.md#variable-declarations`

5. Commit changes

```bash
# Add file contents to index
$ git add .
# Commit changes with message
$ git commit -m "What did you change?" # eg: Message might be "Create Javascript Variables document"
```

7. Push to remote repository

```bash
$ git push origin <branch_name>
# eg: git push origin docs/variables
```

6. Create Pull Request on Github

Reference: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request#creating-the-pull-request
