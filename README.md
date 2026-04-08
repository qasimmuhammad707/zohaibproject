# Hello World CI/CD Test App

Simple Flask "Hello, World!" application with Docker and a GitHub Actions deployment pipeline.

## Project structure

- `app.py` - Flask web server
- `requirements.txt` - Python dependencies
- `Dockerfile` - Container image build definition
- `.github/workflows/deploy.yml` - Build -> push to ECR -> deploy to EC2

## Notes

- Replace placeholders in `.github/workflows/deploy.yml`:
  - `<AWS_ACCOUNT_ID>`
  - `<AWS_REGION>`
- Required GitHub secrets:
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `EC2_HOST`
  - `EC2_USER`
  - `EC2_SSH_KEY`