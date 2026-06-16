# Vercel Deployment Guide

## Deploy Your College Portal on Vercel

Vercel is the easiest and fastest way to deploy Node.js applications.

### Steps to Deploy:

1. Go to https://vercel.com
2. Sign up with GitHub
3. Import your repository
4. Add environment variables:
   - JWT_SECRET: Generate with `openssl rand -base64 32`
   - ENCRYPTION_KEY: Generate with `openssl rand -base64 32`
5. Click Deploy

### Your Live App

Your app will be available at:
https://drcvramancollege-portal.vercel.app

### Environment Variables

Set these in Vercel dashboard:
- NODE_ENV=production
- JWT_SECRET=<your-secret>
- ENCRYPTION_KEY=<your-encryption-key>

### Testing

After deployment:
- Visit: https://drcvramancollege-portal.vercel.app
- Health check: https://drcvramancollege-portal.vercel.app/health

### Continuous Deployment

Every push to GitHub automatically deploys!
