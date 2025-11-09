# Titan AI - A Cloud Security Assistant Using AWS Titan LLM

![Project Screenshot](./assets/titan%20ai%20example%20wide.png)  
*Screenshot of the project interface*

## Overview
The **Cloud Security Assistant** is a web application designed to provide a user-friendly environment for exploring cloud security concepts through natural language queries. The main objective of this project was to deepen my understanding of AWS cloud services, APIs, and cloud security while creating an interactive tool that allows users to ask questions about cloud security topics.

This project builds upon **PartyRock**, an AWS model that generates applications from prompts, by recreating the functionality with full AWS integration, including Lambda, API Gateway, S3, CloudFront, and Amazon Bedrock.

---

## Inspiration

The design of this project was inspired by [Rizki Padilah](https://dribbble.com/shots/23332707-ChaTin-AI-Chatbot-app) and modern, minimalistic web apps that prioritise usability and clarity.

![Design Inspiration Screenshot](./assets/rizki%20design%20inspo.png)

---

## Key Features

- **Static front-end hosted in S3**: HTML, CSS, and JS assets are stored in a bucket and served to users.  
- **API Gateway routing**: Connects the front-end to backend logic via a REST API.  
- **AWS Lambda backend**: Python function handling requests, connecting the front-end to the Amazon Titan language model through Bedrock.  
- **Amazon Bedrock integration**: Provides access to Titan Express for natural language processing.  
- **CloudFront distribution with HTTPS**: Ensures a secure connection for users accessing the site.  
- **Interactive query interface**: Users can ask questions about cloud security topics in a friendly, conversational environment.

---

## Architecture

```plaintext
Browser (Front-end) --> S3 Bucket --> CloudFront (HTTPS) --> API Gateway --> Lambda Function --> Amazon Bedrock (Titan Express) --> Response
```

## Demo

[Watch the demo video](https://youtu.be/KOT6DSRto-c) to see the application in action.

---

## Key Learnings

- Gained hands-on experience with AWS Lambda, API Gateway, S3, CloudFront, and Amazon Bedrock.  
- Learned how to securely connect a static front-end to a dynamic backend.  
- Understood deployment complexities of integrating multiple AWS services.  
- Improved Python API handling and serverless architecture skills.  

---

## Future Improvements

- Add **user authentication and personalised sessions** so that users can save queries or preferences, which may require some minor design adjustments.  
- Extend support for **additional AWS language models** to provide more varied responses and capabilities.  
- Implement **analytics or logging** to track usage patterns and improve the model's responses over time.  
- Optimise **performance and latency** for faster responses from the backend, particularly if multiple users are querying simultaneously.  

---

## Conclusion

This project allowed me to explore **cloud security**, **serverless architecture**, and **AWS integration** in a controlled, user-friendly environment. By building upon PartyRock’s functionality, I created a fully custom web application that demonstrates both practical cloud skills and an understanding of secure API design.