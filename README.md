# cpsc285-autograde (PUBLIC REPO)

Holds the **advisory** sample-feedback runner that student repos call on push.
Everything here is public on purpose. It only ever touches the public sample
tests inside a student's own repo, so there is nothing secret to leak.

- `.github/workflows/sample-feedback.yml` — reusable workflow (`workflow_call`)
- `grade.py` — the same grader script, used here only against public sample data.

**Note: This is not the official graded sample test models.**

### How to use
- Set your org name in `sample-feedback.yml` (the `repository:` for the runner
checkout) and in each student repo's `.github/workflows/feedback.yml`.
