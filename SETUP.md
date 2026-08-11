# Setup Instructions

## 1) Profile repository
Make sure your profile repository is named exactly:

Fath-elpap/Fath-elpap

The repository must be public and contain README.md in the root.

## 2) Add the workflow
Create this path in the profile repository:

.github/workflows/profile-summary-cards.yml

Paste the supplied workflow file there.

## 3) Create the token secret
In GitHub:

Settings → Developer settings → Personal access tokens

Create a token suitable for public profile data.

Then inside the Fath-elpap/Fath-elpap repository go to:

Settings → Secrets and variables → Actions → New repository secret

Name it exactly:

SUMMARY_GITHUB_TOKEN

Paste the token value and save it.

Never paste the raw token into README.md or the workflow YAML.

## 4) Run the workflow once
Open:

Actions → GitHub Profile Summary Cards → Run workflow

When the run finishes successfully, the repository will contain:

profile-summary-card-output/tokyonight/

The GitHub Analytics section in README.md will then display the generated cards.

## 5) Replace project placeholders
Search README.md for:

ADD_PROJECT_LINK

Replace each one with the correct GitHub repository URL.

## 6) Optional email
Search for:

YOUR_EMAIL

Replace it with your real email and remove the surrounding HTML comment markers if you want the email badge visible.
