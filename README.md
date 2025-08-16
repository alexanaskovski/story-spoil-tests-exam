# Story Spoiler – RestSharp API Tests

## How to run locally
```bash
dotnet test ./StorySpoiler.ApiTests/StorySpoiler.ApiTests.csproj
```
Optionally set environment variables to use an existing account:
- `STORY_USER`
- `STORY_PASS`

If not set, the tests will create a random user and then authenticate.

## CI
A GitHub Actions workflow is included at `.github/workflows/ci.yml`.
It restores, builds and runs tests on every push to `main`.
To use an existing account in CI, add repository secrets `STORY_USER` and `STORY_PASS`.