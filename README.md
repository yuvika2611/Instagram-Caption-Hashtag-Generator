# My AI Agent

**My Ai Agent** is an advanced AI-driven Instagram content automation workflow designed to simplify and supercharge your social media marketing efforts. The project integrates several powerful tools to automate viral caption and hashtag generation, content management, and posting strategies.

## What This Project Does

- Uses **PhantomBuster** to scrape viral Instagram post data (like captions, comments, engagement metrics).
- Imports scraped data manually or automatically into **Airtable**, which acts as the central content database.
- Filters and manages posts in Airtable based on status and engagement.
- Uses **n8n** workflow automation to:
  - Generate creative, niche-targeted Instagram captions with **OpenAI GPT**.
  - Generate relevant hashtags for each post.
  - Update Airtable with captions, hashtags, and post statuses.
  - Prepare data for manual or automated posting.
- Planned extensions include automatic posting and cross-platform content repurposing (Instagram + YouTube).

## How It Works

1. **Data Collection:** PhantomBuster scrapes Instagram viral posts and exports the data as CSV.
2. **Data Management:** You import the CSV into Airtable, where posts are tagged and filtered for processing.
3. **Caption & Hashtag Generation:** n8n triggers AI models to create viral captions and hashtags tailored to your niche.
4. **Workflow Automation:** The system updates Airtable statuses to track progress and organize posting schedules.
5. **(Future) Automated Posting:** Integration with Instagram’s API or third-party tools to schedule and publish posts automatically.

## Tools and Technologies

- [PhantomBuster](https://phantombuster.com/) – for Instagram data scraping
- [Airtable](https://airtable.com/) – database and content management
- [n8n](https://n8n.io/) – workflow automation platform
- [OpenAI GPT](https://openai.com/) – AI text generation for captions and hashtags
- JSON – workflow export format for easy import/export

## How to Use

- Import the exported JSON workflow into your n8n instance.
- Connect your OpenAI API key and Airtable API key in n8n credentials.
- Set up your Airtable base with required tables and views as per the workflow.
- Use PhantomBuster to scrape Instagram viral posts and import them into Airtable.
- Run the workflow regularly (via cron or triggers) to generate content automatically.
- Customize prompts and workflow settings for your specific niche and audience.

## License

This project is open for personal and commercial use. Please credit the original author if you share or modify the workflow.

---

*Created and maintained by Yuvika Singh*
