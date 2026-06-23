# gha-badge

GitHub Action to manage shields.io badge lifecycle using:
- [gha-setup-shields](https://github.com/albr21/gha-setup-shields)
- [gha-create-shields-badge](https://github.com/albr21/gha-create-shields-badge)
- [gha-git-push](https://github.com/albr21/gha-git-push)

## Usage

```yaml
steps:
  - name: Manage badge
    uses: albr21/gha-badge@1.0.0
    with:
      label: Build
      message: Passing
      color: green
      target-path: path/to/badge.svg
      target-repo: owner/repo
      target-branch: main
      commit-message: "Add build badge"
      commit-author-name: "github-actions[bot]"
      commit-author-email: "github-actions[bot]@users.noreply.github.com"
      auth-method: token
      github-token: ${{ secrets.GITHUB_TOKEN }}
```

For more information about input options, check out the [action.yml](action.yml) file.

## Contributing

Check out the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
