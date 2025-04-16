# Upwork-project Workflow on n8n Documentation

## Who is this for?
This workflow is designed for iSemantics to automate the extraction and scoring of Upwork job posts based on specific skill sets, budget attractiveness, and client history.

## What problem is this workflow solving?
This workflow addresses the challenge of quickly identifying and scoring job opportunities on Upwork that align with iSemantics' skills and budget preferences, enabling more efficient job applications.

## What this workflow does
- Retrieves job posts from a PostgreSQL database.
- Extracts relevant skills from job descriptions, categorizing them into predefined groups such as Programming, NLP & RAG, etc.
- Scores job posts based on budget attractiveness, client history, post freshness, and skill relevance.
- Generates personalized cover letters tailored to the requirements of high-scoring job posts.
- Outputs results to Google Sheets for easy reference and tracking.

## Setup
1. **Database Credentials**: Set up your PostgreSQL database connection with the necessary credentials to access job data.
2. **OpenAI API**: Integrate your OpenAI API credentials to utilize AI models for skill extraction and cover letter generation.
3. **Google Sheets**: Connect your Google Sheets account to store and manage the output data.
4. **Gmail Integration**: Link your Gmail account for email functionalities if needed.

## How to customize this workflow to your needs
- Modify the filtering criteria in the `GetTabelRecords` node to adjust the job selection parameters, including budget and processing status.
- Update the skill extraction logic in the `OpenAI Chat Model` and `ExtractSkills` nodes for different categorization as per your needs.
- Adjust score weightings in the `ScoreJobPost` by redefining the criteria for scoring jobs based on your specific requirements.
- Personalize the cover letter templates in the `GenerateCoverLetter` node to reflect your unique selling points or specific project experiences. 

This workflow was created using n8n and is effective for freelancers seeking to optimize their Upwork job application process.
