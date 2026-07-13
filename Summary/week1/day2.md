
## 13. LLM Engineering Building Blocks: Models, Tools & Techniques
In this lecture the instructor focuses on the foundational aspects of LLM engineering. Here’s a summary of the key points covered:

Recap of Previous Day: The session begins with a review of the previous day's activities that included working with Olama, understanding prompts, and a summarization use case.
Models: Different types of models are discussed, covering both open-source and closed-source options, along with multimodal models capable of generating images and audio. The importance of choosing the right model for specific tasks is emphasized.
Tools and Frameworks: Several tools and libraries to be used throughout the course are introduced, such as Hugging Face, Long Chain, Gradio, Weights and Biases, and Modal.
Techniques: Various techniques for utilizing these models and tools are explored, including API calls, multi-shot prompting, fine-tuning, and agentization.
The instructor encourages engagement from participants of all skill levels, emphasizing practical application. Self-study guides are provided for additional support, and students are urged to actively work on coding exercises and share their progress on platforms like LinkedIn to foster community engagement.
Overall, the lecture aims to equip students with the skills necessary for effective use of LLMs, encouraging persistence and active participation throughout the course.


## 14. Your 8-Week Journey: From Chat Completions API to LLM Engineer

This lecture outlines an engaging eight-week journey aimed at transforming participants into LLM engineers. Here's a breakdown of what to expect:

Week 1: Focus on foundational knowledge and the Chat Completions API from OpenAI.
Week 2: Exploration of various frontier models and APIs, including advanced concepts like multimodality.
Week 3: Engagement with open-source models using Hugging Face, with an emphasis on building innovative projects.
Week 4: Learning to select the appropriate LLM for applications like code generation and porting.
Week 5: Introduction to Retrieval-Augmented Generation (RAG), where participants will create a knowledge worker expert for processing extensive documents.
Week 6: Focus on fine-tuning models and essential data science skills like data scrubbing and curation.
Week 7: Fine-tuning an open-source model for a specific business task, leading to an unexpected outcome.
Week 8: Integration of all learnings into the development of a generative platform that addresses a commercial problem.
Throughout this journey, participants will have access to engaging content, tools, and resources, including a code cookbook to support their projects.


## 15. Day 2 - Frontier Models: OpenAI GPT, Claude, Gemini & Grok Compared

In the previous lecture, we focused on frontier models in generative AI, distinguishing between closed source and open source models. The main points included:

Closed Source Models: These are typically developed by major companies (Frontier Labs) and require payment for access due to high development costs. Notable examples include:

OpenAI's GPT: With GPT 5 being the latest version, following the popular ChatGPT release in late 2022.
Claude by Anthropic: Known for its powerful versions like Haiku, Sonnet, and Opus; Claude is also used in coding platforms.
Google's Gemini: This evolved from the earlier Bard model, with Gemini 2.5 Pro currently available and a new version, Gemini 3, expected soon.
Grok by X.ai: Recognized as part of the big four frontier models alongside GPT, Claude, and Gemini.
Comparison of Models: The lecture emphasized understanding the capabilities of these models and how they compare to one another, while acknowledging that open source models will be discussed in later sessions.

The session concluded with a promise to delve into how to choose the right model for specific tasks in the upcoming weeks.


## 16. Open-Source LLMs: LLaMA, Mistral, DeepSeek, and Ollama
It covers various open-source models, including LLaMA, Mistral, DeepSeek, and Ollama, focusing on their characteristics, applications, and differences. Here’s a detailed summary:
LLaMA Models: The chapter begins with LLaMA (Large Language Model Meta AI) versions, discussing LLaMA 3.2 and its 3 billion parameters, which is notable for being easier to run on local computers. More powerful versions like LLaMA 3.1 come in sizes of 8 billion, 70 billion, and the 405 billion version, which competes with closed-source models in capabilities. The sheer scale of parameters in these models—up to 10 trillion—highlights their complexity compared to traditional models.
Mistral: This section introduces the Mistral model from the French company Mistral, characterized as a mixture of experts model. It effectively channels queries to specialized smaller models within its framework to provide context-specific answers, showcasing innovative approaches in open-source LLM development.
DeepSeek: The chapter briefly touches on DeepSeek, discussing its contribution to the realm of open-source models. While specific details may not have been outlined, it positions itself alongside other prominent models, emphasizing collaboration and experimentation in the field.
Ollama: Ollama is introduced as a wrapper project facilitating the use of various small-scale LLMs, including Qwen 3.4B and Qwen 2.5 coder. The discussion around Ollama stresses the importance of experimentation with different models for personal and professional projects, highlighting its practical implications in the LLM engineering domain.
Experiments and User Experiences: The instructor shares personal experiences with different models, indicating that while Qwen 2.5 shows great promise across various languages, certain models excel in specific tasks like explanation. Encouraging learners to explore and share their findings not only fosters community but also enhances understanding of which models are best suited for particular applications.
Conclusion: The chapter concludes by emphasizing the importance of hands-on experimentation with open-source models to find the best fit for specific problems, an essential skill for aspiring LLM engineers.
This chapter serves as a valuable resource for understanding the landscape of open-source language models and encourages learners to actively engage with and evaluate these powerful tools.

## 17.  Chat Completions API: HTTP Endpoints vs OpenAI Python Client
This chapter focuses on the Chat Completions API, a key method for interacting with large language models like OpenAI's GPT-5. Here’s a detailed summary:
Setting Up the Environment: The instructor begins by guiding you through setting up your Python environment, underscoring the importance of choosing the correct kernel for running code.
Introduction to Chat Completions API: The Chat Completions API is presented as a standard mechanism for engaging with LLMs, where you provide conversation context, and the model predicts the next message—similar to how predictive text works.
Understanding API Endpoints: The lecture highlights the importance of API endpoints, which are URLs used to make requests to an API, specifically detailing the OpenAI endpoint for chat completions.
Making API Requests: The process of formulating an API request is explained, including:

Setting HTTP headers
Constructing a JSON payload that includes the model and user's message
An example illustrates how to request a fun fact from the model, demonstrating request formatting and JSON response handling.
Challenges with Manual Requests: The potential difficulty in manually crafting HTTP requests and navigating JSON responses is acknowledged, which can be cumbersome for users.

Using the OpenAI Python Client Library: To simplify API interactions, the OpenAI Python client library is introduced. This library abstracts away the complexities of sending HTTP requests and handling JSON, allowing for cleaner and more intuitive Python coding.
Reassurance on Library Use: The instructor emphasizes that the library is open source and user-friendly, serving merely to wrap the HTTP request process.
Overall, this chapter provides foundational knowledge and practical tools to effectively use the Chat Completions API along with the OpenAI Python client library. If you need more details or have specific questions about a topic, feel free to ask!

## 18.  Using the OpenAI Python Client with Multiple LLM Providers
This chapter focuses on utilizing the OpenAI Python client to interact with multiple large language model (LLM) providers. Here’s a detailed summary:
Creating the OpenAI Python Client: The lecture begins by showing how to create an OpenAI Python client that automatically retrieves the OpenAI API key from environment variables, simplifying setup.
Making API Requests: The speaker demonstrates how to make a POST request to the chat completions endpoint. They explain how to pass parameters like the model and messages without the need for manual JSON crafting, which enhances usability.
Simplicity and Elegance: Emphasis is placed on the elegance and simplicity of the OpenAI library. It acts as a wrapper for making HTTP calls to the API, making the coding experience more intuitive.
Interoperability Among LLM Providers: The lecture discusses how other LLM providers, such as Google’s Gemini model, have created compatible endpoints. This allows users to easily switch between different providers as they often adopt similar endpoint structures.
Configuring for Different Providers: The speaker explains how to configure the library to connect to these alternative endpoints, which involves specifying the base URL and API key for the selected model.
Practical Example with Gemini: A practical demonstration is gßßiven on setting up the Gemini client using the same structure as the OpenAI client, showing that users can change the model name and base URL to switch providers seamlessly.
Retrieving Fun Facts: The lecture concludes with a demonstration of retrieving fun facts from both OpenAI and Gemini, showcasing the ease of switching between models while maintaining a consistent coding approach.
Overall, the chapter provides valuable insights into the interoperability of LLM APIs and the practical use of the OpenAI Python client. If you have any specific questions or need further elaboration on any point, feel free to ask!

## 19.  Running Ollama Locally with OpenAI-Compatible Endpoints