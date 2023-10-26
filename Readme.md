# Git Commit with Flag

This script, `commitWithFlag`, is a handy tool for making Git commits with predefined commit types and optional issue tags. It simplifies the process of committing changes in your Git repository by allowing you to specify the type of commit and an associated issue tag. If no issue tag is provided, it defaults to "no-id."

## Usage

```shell
gitp -f|-fx|-r|-m|-a 'commit_message' ['issue_tag']
```

- `-f`: Use this flag for a **feature** commit.
- `-fx`: Use this flag for a **bug fix** commit.
- `-r`: Use this flag for a **refactoring** commit.
- `-m`: Use this flag for a **merge** commit.
- `-a`: Use this flag for an **addition** commit.

Replace `'commit_message'` with a concise message that describes your commit.

Optionally, you can specify an issue tag, which is useful for tracking and associating commits with specific issues or tasks. If no issue tag is provided, it defaults to "no-id."

## Examples

### Feature Commit
```shell
gitp -f 'Implement new user registration'
```

### Bug Fix Commit
```shell
gitp -fx 'Fix login page validation issue' 'ISSUE-123'
```

### Refactoring Commit
```shell
gitp -r 'Rewrite authentication module for clarity'
```

### Merge Commit
```shell
gitp -m 'Merge branch "feature-branch"'
```

### Addition Commit
```shell
gitp -a 'Add new documentation files'
```

## Additional Git Aliases

In addition to the `commitWithFlag` function, this script also provides a couple of useful Git aliases:

- `gitp`: An alias for the `commitWithFlag` function, making it easier to commit using the specified flags.

- `gita`: An alias for `git add .`, simplifying the process of adding all changes in the current directory to the staging area.

Feel free to customize these aliases or integrate them into your Git workflow as needed.

## Author

This script was created to simplify Git commits by [Your Name] (Replace with your name).

## License

This script is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.