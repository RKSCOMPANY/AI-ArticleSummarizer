# AI-ArticleSummarizer

AI-Article Summarizer

The AI-Article Summarizer is a Python-based tool designed to efficiently summarize articles from the web. This project leverages web scraping, prompt engineering, and the power of OpenAI's GPT-4 to deliver concise and accurate summaries of lengthy articles. Here’s an in-depth look at the main steps involved:

Scraping the Article from the Given Link:

The first step involves fetching the full text of the article from the provided URL. This is accomplished using web scraping libraries such as BeautifulSoup and requests. The scraper navigates through the HTML structure of the webpage to extract the main content of the article while filtering out irrelevant information like advertisements and navigation links.
Preparing the Template for the Prompt:

After successfully scraping the article, the next step is to prepare a structured template for the prompt. This template will guide the AI in generating the summary. The template typically includes key components such as the title, author (if available), and the main body of the article. It also sets the context for the AI, specifying that the task is to summarize the given content.
Setting Up the OpenAI API and Loading the Model GPT-4:

Before generating the summary, the OpenAI API needs to be set up. This involves installing the OpenAI Python client library and configuring it with the necessary API key. Once the setup is complete, the GPT-4 model is loaded and initialized, ready to process the prompts and generate the summary.
Generating and Printing the Summary of the Article Using Two Prompts:

To ensure a high-quality summary, two different prompts are used to generate the final output. The first prompt might focus on capturing the main points and key takeaways of the article, while the second prompt could be designed to provide a more detailed and nuanced summary. Both summaries are then printed, allowing for a comparison and selection of the most effective summary.
