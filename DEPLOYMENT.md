# 🚀 Deployment Guide

## Quick Deploy Options

### 1. Vercel (Recommended)
```bash
npm install -g vercel
vercel
```
- Free tier available
- Automatic HTTPS
- Global CDN
- Easy environment variables setup

### 2. Railway
```bash
# Connect your GitHub repo to Railway
# Or use Railway CLI
npm install -g @railway/cli
railway login
railway deploy
```

### 3. Render
- Connect your GitHub repo to Render
- Uses `render.yaml` configuration
- Free tier with limitations

### 4. Heroku
```bash
heroku create your-app-name
git push heroku main
```

## Environment Variables Setup

For any platform, you'll need to set these environment variables:

```env
GEMINI_API_KEY=your-gemini-api-key
GEMINI_MODEL=gemini-pro
PRIMARY_INDUSTRY=professional
CAMPAIGN_STYLE=balanced
NODE_ENV=production
PORT=3000
```

## Pre-deployment Checklist

- [ ] Get Gemini API key
- [ ] Test locally with `npm run web`
- [ ] Set up environment variables on hosting platform
- [ ] Configure custom domain (optional)
- [ ] Set up monitoring/analytics (optional)

## Post-deployment

1. Test the live URL
2. Create your first campaign
3. Monitor performance and usage
4. Set up backups for important data

## Troubleshooting

- **Build fails**: Check Node.js version compatibility
- **App crashes**: Verify all environment variables are set
- **Slow performance**: Consider upgrading to paid tier
- **API errors**: Verify Gemini API key and quotas