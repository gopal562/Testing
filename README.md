# Hello World Node.js with CI Pipeline

This project contains a simple Node.js Hello World application with a GitHub Actions CI pipeline.

## Project Structure

- `server.js` - Main HTTP server that responds with "Hello World!"
- `test.js` - Simple test file
- `package.json` - Node.js project configuration
- `.github/workflows/pipeline.yml` - GitHub Actions CI pipeline

## Running Locally

1. Start the server:
   ```bash
   npm start
   ```

2. Visit `http://127.0.0.1:3000/` in your browser or use curl:
   ```bash
   curl http://127.0.0.1:3000
   ```

## Running Tests

```bash
npm test
```

## CI Pipeline

The GitHub Actions pipeline automatically runs on every push to any branch and includes:

- **Multi-version testing**: Tests on Node.js 18.x and 20.x
- **Automated testing**: Runs npm test on every push
- **Artifact upload**: Saves the application files

## Setting Up GitHub

1. Initialize git repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit with Node.js app and CI pipeline"
   ```

2. Create a new repository on GitHub

3. Push to GitHub:
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git branch -M main
   git push -u origin main
   ```

4. The pipeline will automatically run on push!

## Viewing Pipeline Results

After pushing to GitHub:
1. Go to your repository on GitHub
2. Click the "Actions" tab
3. You'll see your pipeline running or completed
4. Click on any workflow run to see detailed logs
