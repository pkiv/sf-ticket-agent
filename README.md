# 🤘 SF Parking Ticket Payment Automation

Welcome! This project demonstrates how to automate parking ticket payments using [Stagehand](https://github.com/browserbase/stagehand).

## About This Project

This automation script helps you pay parking tickets on the San Francisco Municipal Transportation Agency website. It uses Stagehand, an SDK built on top of [Playwright](https://playwright.dev/) that provides AI-powered automation capabilities.

## Getting Started

1. Run `npx create-browser-app` to create a new project:

   ```bash
   npx create-browser-app@latest sf-parking-payment
   ```

2. Copy `.env.example` to `.env` and update with your credentials:

   ```bash
   cp .env.example .env
   ```

   Required credentials in .env:

   ```
   BROWSERBASE_PROJECT_ID="YOUR_BROWSERBASE_PROJECT_ID"
   BROWSERBASE_API_KEY="YOUR_BROWSERBASE_API_KEY"
   OPENAI_API_KEY="THIS_IS_OPTIONAL_WITH_ANTHROPIC_KEY"
   ANTHROPIC_API_KEY="THIS_IS_OPTIONAL_WITH_OPENAI_KEY"
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Run the script:

   ```bash
   npx tsx index.ts
   ```

## What This Script Does

1. Navigates to the SF Municipal Transportation Agency payment portal
2. Enters license plate information
3. Selects tickets to pay
4. Fills out payment information using Stagehand's AI-powered form filling

Note: This is a demo script using test credit card numbers. Please update the payment information with real data when using it.
