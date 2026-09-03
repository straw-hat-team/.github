# Contributing

Thank you for investing your time in contributing to our project!

Read our [Code of Conduct](./CODE_OF_CONDUCT.md) to keep our community
approachable and respectable.

Read our [AI Contribution Policy](./AI_POLICY.md) before contributing with the
help of AI tools like agents and LLMs.

## Commits

We follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

```text
<type>(<optional scope>): <subject>
```

We use three types:

- `feat` for a backwards compatible addition, which bumps the `MINOR` version.
- `fix` for a backwards compatible fix, which bumps the `PATCH` version.
- `chore` for everything else, including documentation, tests, refactors, and continuous
  integration. It releases nothing.

Mark a breaking change with a `!` after the type, as in `feat!:` or `fix!:`, which bumps the `MAJOR`
version. Read our [Versioning Policy](./VERSIONING.md) to know what counts as breaking.

The subject line drives the release, so keep the type accurate.

## Sign your work

Every commit needs a [Developer Certificate of Origin](https://developercertificate.org) sign-off,
which states that you wrote the change or otherwise have the right to submit it:

```shell
git commit -s
```

That appends a `Signed-off-by` trailer using your `user.name` and `user.email`. To fix commits you
already made, run `git rebase --signoff <base>` and force push your branch.

## Pull Request

When you're finished with the changes, create a pull request, also known as a PR.

- Don't forget to [link PR to issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
  if you are solving one.
- Enable the checkbox to [allow maintainer edits](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
  so the branch can be updated for a merge.
- We may ask for changes to be made before a PR can be merged, either using [suggested changes](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request)
  or pull request comments. You can apply suggested changes directly through the UI. You can make any other changes in your fork, then commit them to your branch.
- As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
- If you run into any merge issues, checkout this [git tutorial](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)
  to help you resolve merge conflicts and other issues.
