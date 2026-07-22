# Practice CI/CD Project

A deliberately simple calculator app used to learn GitHub Actions, one concept at a time.
Each milestone below adds exactly one new CI/CD concept to this repo.

## Milestones

- [x] **0. Baseline** — calculator functions + pytest tests, no Actions yet
- [x] **1. Basic CI** — workflow runs on push/PR, installs deps, runs tests
- [ ] **2. Branch protection** — `main`/`develop` branches, PR + passing CI required to merge
- [ ] **3. Secrets** — a fake API key stored as a GitHub Secret, used in a step
- [ ] **4. Artifacts** — upload the test/coverage report so it survives after the job ends
- [ ] **5. Quality gate** — `flake8` linting as a required check that can block a PR
- [ ] **6. Environments & approval** — a "deploy" job gated behind manual approval
- [ ] **7. Reusable workflow** — extract build+test into its own file, call it from `ci.yml`
- [ ] **8. Matrix builds** — test against Python 3.10, 3.11, and 3.12 in parallel
- [ ] **9. Concurrency control** — cancel an in-progress run if a newer push arrives
- [ ] **10. Docker** — build an image and push it to GitHub Container Registry

## Running locally

```bash
pip install -r requirements.txt
pytest -v
```
