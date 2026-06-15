# Maintainer Workflow

This project is maintained as a public, static educational utility for creating printable vertical Japanese kanji worksheets. It is intentionally distributed as a single HTML file so teachers and parents can use it without a backend service or account.

Live site: https://gahiru.github.io/kanji-test-maker-tate/

## Project Role

- Helps teachers and parents prepare vertical kanji tests, answer sheets, and reading tests from CSV data.
- Keeps worksheet data local in the browser, which is important for classroom and home-learning privacy.
- Supports legacy CSV data while improving the print layout for real Japanese vertical writing.

## Current Maintenance Signals

- The project is public and licensed under the MIT License.
- The tool is available as a GitHub Pages site and as a single `index.html` file.
- `main` is protected through a GitHub ruleset that requires pull requests before merging, blocks force pushes, and restricts deletions.
- Bug reports, classroom/home-learning feedback, and release checks have GitHub issue and pull request templates.
- Releases are documented in `CHANGELOG.md`.
- Changes that affect layout are verified with browser previews and PDF-oriented checks before release.

## How Codex Helps Maintenance

Codex is especially useful for this repository because the hardest parts are layout-sensitive and review-heavy rather than large-scale backend work.

Planned and current maintainer workflows include:

- Issue triage: summarize bug reports from teachers or parents and turn them into reproducible test cases.
- PR review: inspect single-file HTML, CSS, and Canvas changes for behavior regressions.
- Visual checks: run browser previews for kanji tests, answer sheets, and reading tests after layout changes.
- Release workflow: prepare changelog entries, PR summaries, and manual verification notes.
- Privacy and security review: check that CSV handling and PDF generation stay local to the browser and do not introduce unnecessary external services.
- Documentation: keep README, contribution guidance, and user-facing instructions aligned with the current release.

## Release Verification Checklist

Before updating `main`, verify the following where relevant:

- Sample CSV loads successfully.
- 10-question output renders as 5/5.
- 11-question output renders as 6/5.
- 12-question output renders as 6/6.
- Kanji test, answer sheet, and reading test previews render correctly.
- Punctuation placement is visually checked after parentheses, hiragana, and kanji.
- PDF save or browser print workflow still works.
- Browser console has no unexpected errors.
- README and `CHANGELOG.md` describe the released behavior accurately.

## Roadmap

- Add lightweight regression screenshots or documented manual checks for PDF output.
- Expand sample CSV data based on real classroom and home-learning feedback.
- Continue improving Japanese vertical-writing details without making the tool harder to run locally.
- Use public demo feedback to prioritize UI improvements.