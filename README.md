# Serverless Function Demo

A simple demonstration of serverless architecture using Vercel.

## 🚀 Live Demo

**URL:** https://serverless-demo-kappa.vercel.app

**API Endpoint:** https://serverless-demo-kappa.vercel.app/api/hello

## Screenshot

![Serverless Demo](screenshots/demo.png)

## Project Structure

```
serverless-demo/
├── api/
│   └── hello.js      # Serverless function
├── index.html        # Frontend page
├── package.json
└── README.md
```

## How Serverless Works

- **No server management**: You don't need to maintain or scale servers
- **Pay per execution**: Code runs only when invoked
- **Auto-scaling**: Handles traffic spikes automatically
- **Fast deployment**: Deploy in seconds

## Deployment Steps

### Prerequisites
1. Create a [Vercel account](https://vercel.com/signup)
2. Install Vercel CLI: `npm install -g vercel`

### Deploy

1. Navigate to the project folder:
   ```bash
   cd serverless-demo
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy the project:
   ```bash
   vercel
   ```

4. For production deployment:
   ```bash
   vercel --prod
   ```

### Access Your Function

After deployment, your function will be available at:
- `https://your-project.vercel.app/api/hello`

## Local Development

Run locally with:
```bash
npm run dev
```

Then visit: `http://localhost:3000`

## API Endpoint

### GET /api/hello

Returns a JSON response:

```json
{
  "message": "Hello from serverless!",
  "timestamp": "2024-01-15T10:30:00.000Z",
  "method": "GET"
}
```
