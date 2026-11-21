# Contributing to SupplyLens

Thank you for your interest. This guide applies to every SupplyLens project under this account.

## Ways to help

- **Ask a question or share an idea** in [Discussions](https://github.com/MDABDURRAUF/supplylens/discussions).
- **Report a bug** with the bug report template in the project it concerns.
- **Suggest a feature** with the feature request template.
- **Improve the documentation**: unclear wording, a missing example, a broken link.
- **Share domain knowledge**: if you work in procurement, logistics or planning, tell us where an output does not match how the decision is really made.
- **Send code**: issues labelled `good first issue` are a good place to start.

## Setting up

Each project is a standard Python package and needs Python 3.10 or later.

```bash
git clone https://github.com/MDABDURRAUF/<project>.git
cd <project>
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -e ".[app,dev]"
pytest
```

All tests should pass before you change anything. If they do not, please open an issue.

## Making a change

1. For anything larger than a small fix, open an issue or discussion first so the approach can be agreed before you spend time on it.
2. Fork the repository and create a branch from `main`.
3. Keep the change focused: one topic per pull request.
4. Add or update tests for behaviour you change.
5. Run `pytest` and make sure it passes.
6. Open a pull request that says what changed and why. Link the issue if there is one.

## What a good change looks like

- **Honest about data.** Sample data is simulated and must stay labelled as simulated. Do not add figures about real companies, carriers or markets without a source that can be checked.
- **No leakage.** A feature or forecast may only use information that was available at the time of the decision. Changes to model inputs need a test showing this.
- **Explained.** A new output should say what it means and what its limits are, in the README or in the dashboard next to the number.
- **Plain language.** Dashboards and reports are read by planners, not only by data scientists.
- **Small dependencies.** New packages need a clear reason.

## Reporting a security problem

Please do not open a public issue. Use "Report a vulnerability" on the Security tab of the repository.

## Conduct

Everyone taking part is expected to follow the [code of conduct](CODE_OF_CONDUCT.md).

## License

The projects are released under the MIT License. By contributing you agree that your contribution is released under the same license.
