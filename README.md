
# Contributing to This Project

We welcome contributions from everyone! To ensure a smooth and collaborative development process, please follow these guidelines.

## Branching Strategy

- It is **mandatory** that all contributions are made on a separate branch.  
- Direct pushes to the **main** branch are strictly prohibited.

## Branch Naming Convention

Please name your branches using the following format:

```

dev/{your\_github\_username}/{feature\_or\_bugfix\_description}

````

### Examples:

- For a new feature by user `reza`:  
  `dev/reza/add-user-authentication`

- For a bug fix by user `jane-doe`:  
  `dev/jane-doe/fix-login-bug`

- For a small improvement:  
  `dev/john-smith/improve-error-messages`

### How to create your branch:

```bash
git checkout main
git pull origin main
git checkout -b dev/your_github_username/your-feature-name
````

## Getting Started

1. **Fork the repository:**
   Click the "Fork" button at the top right of this repository.

2. **Clone your forked repository:**

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME
```

3. **Add the original repository as an upstream remote:**
   This allows you to fetch changes from the main project.

```bash
git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY_NAME.git
```

4. **Keep your main branch updated:**
   Regularly pull changes from the upstream main branch.

```bash
git checkout main
git pull upstream main
```

## Making Changes

1. **Create a new branch:** As per the branching strategy above.

```bash
git checkout -b dev/your_github_username/your-feature-name
```

2. **Make your changes:**
   Write your code, tests, and documentation.

3. **Commit your changes:**

* Write clear, concise, and descriptive commit messages.
* Start your commit message with a type (e.g., `feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `test:`, `chore:`).

**Good example:**
`feat: Implement user profile page`

**Bad example:**
`fix bug`

```bash
git add .
git commit -m "feat: Your descriptive commit message"
```

4. **Push your branch to your forked repository:**

```bash
git push origin dev/your_github_username/your-feature-name
```

## Submitting a Pull Request (PR)

Once your changes are ready and pushed to your branch:

1. Go to your forked repository on GitHub.
2. Click on **Compare & pull request** next to your newly pushed branch.
3. Fill out the Pull Request template:

   * Provide a clear and concise title for your PR.
   * Describe the changes you've made and why they are necessary.
   * Reference any related issues (e.g., `Closes #123`, `Fixes #456`).
4. Ensure all checks (CI/CD, tests) pass.
5. Request a review: Once submitted, a maintainer will review your PR. Be prepared to address any feedback or make further changes.

## Code Style

* Adhere to the existing code style of the project.
* Run any linters or formatters if configured (e.g., Prettier, ESLint).

## Reporting Bugs and Suggesting Features

If you find a bug or have a feature request, please open an issue on the GitHub issue tracker. Provide as much detail as possible.

