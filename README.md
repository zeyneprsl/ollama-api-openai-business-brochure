# ollama-api-openai-business-brochure
This code is an application design that analyzes a website and uses the information it collects from there to create brochures for companies. Here are the general functions of the code:

Website Data Collection:

The Website class sends an HTTP request to the website using the given URL and collects the content of the page (text and links).
Selecting Links:

The get_links function collects all the links on the web page and presents them as a prompt for the user to choose which links are more suitable for the brochure. It expects a response from the user in JSON format.
Creating Descriptions and Brochure Content:

With the connection information received from the user, the get_all_details function collects the web page content and important links extracted from this content.
The create_brochure and stream_brochure functions create a brochure about the company using information obtained from the company's landing page and other important pages.
AI Interaction with OpenAI (or Ollama):

In this process, a connection is established with OpenAI or Ollama, and a system message and user message are passed to OpenAI's or Ollama's model. The model creates a brochure outline using this data.
Viewing Results:

The results are displayed either as a completed text or as a stream in Markdown format.
