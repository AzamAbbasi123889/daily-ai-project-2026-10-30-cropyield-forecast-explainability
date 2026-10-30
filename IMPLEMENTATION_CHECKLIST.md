# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] POST /forecast returns HTTP 200
- [ ] MAE on held‑out test set <= 15% of average yield
- [ ] Response includes fields: forecast, lower_ci, upper_ci, explanation
- [ ] Explanation length 2‑4 sentences
- [ ] Mentions at least two weather variables and one satellite metric
- [ ] UI shows numeric forecast, confidence band and explanation
- [ ] No client‑side errors in Chrome console
- [ ] Set up repo, Docker, CI
- [ ] Ingest a 3‑month sample of weather, soil, NDVI for 5 regions
- [ ] Implement preprocessing scripts
- [ ] Train a baseline TFT on DVC tracked data
- [ ] Unit tests for preprocessing functions (pytest)
- [ ] Model inference test with dummy input (assert shape)
- [ ] API contract tests using FastAPI TestClient (status codes, schema)
- [ ] End‑to‑end test: POST /forecast → verify JSON contains all fields
- [ ] React component snapshot tests
- [ ] Dockerfile for backend, Dockerfile for frontend
- [ ] docker‑compose.yml orchestrates postgres, api, frontend
- [ ] CI workflow builds images, runs tests, pushes to Docker Hub
- [ ] Deploy on Fly.io (free tier) or Render with automatic HTTPS

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
