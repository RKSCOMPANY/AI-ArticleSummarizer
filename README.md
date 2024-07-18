# AI-ArticleSummarizer

The AI-Article Summarizer is a Python-based tool designed to efficiently summarize articles from the web. This project leverages web scraping, prompt engineering, and the power of OpenAI's GPT-4 to deliver concise and accurate summaries of lengthy articles. Here’s an in-depth look at the main steps involved:

1) Scraping the Article from the Given Link:

The first step involves fetching the full text of the article from the provided URL. This is accomplished using web scraping libraries such as BeautifulSoup and requests. The scraper navigates through the HTML structure of the webpage to extract the main content of the article while filtering out irrelevant information like advertisements and navigation links.

2) Preparing the Template for the Prompt:

After successfully scraping the article, the next step is to prepare a structured template for the prompt. This template will guide the AI in generating the summary. The template typically includes key components 

"""You are an advanced AI assistant that summarizes online articles into bulleted lists.

Here's the article you need to summarize.

Now, provide a summarized version of the article in a bulleted list format.

""" 
specifying that the task is to summarize the given content.

3) Setting Up the OpenAI API and Loading the Model GPT-4:

Before generating the summary, the OpenAI API needs to be set up. This involves importing the OpenAI  and configuring it with the necessary API key. Once the setup is complete, the GPT-4 model is loaded and initialized, ready to process the prompts and generate the summary.


4) Generating and Printing the Summary of the Article Using Two Prompts:

To ensure a high-quality summary, two different prompts are used to generate the final output. The first prompt might focus on capturing the main points and key takeaways of the article, while the second prompt could be designed to provide a more bulleted summary. Both summaries are then printed, allowing for a comparison and selection of the most effective summary.
