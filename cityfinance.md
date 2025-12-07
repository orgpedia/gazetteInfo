# Chatting with cityfinance.in data


The goal of this  project is to build a chatting application that will allow users to ask relevant questions on the city finance data. The questions will be asked in plain English and the responses will also be returned in plain English, with some summarised tabular data. Given that the cityfinance data is primarily tabular the chatting application will be required to perform mathematical operations on the data to answer the relevant questions and will require an integration of language model with a data processing system.

Given that the problem of chatting with tabular data is still a research problem, we will be executing the project in multiple phases, the initial phase will focus on the viability of the technology and the later phases will focus on different user personas and deploying the applicaton.

## Why build a chatting application
Chatting or a chatbot is a paradigm which is understood to all - with the prevalance of WhatsApp every person knows how to type their questions and get a response back, whether from a human or a machine. Furthermore, ChatGPT has demonstrated that even complex topics can be understood using a chatting interface. The user can tune the scope and complexity of the response as per their current need, makeing the interface very powerful for a wide range of users. Chatting is especially useful where the user has no background knowledge of the data or the inherent relationsips between the data elements. Though dashboards are still a preferred way for advanced analytics, chatting could be seen as a gateway to the dashboards.

## Requirements
1. Chatting application should be able to understand all the relevant questions that can be answered on the dataset. This is very different from the customer service chatbots that are very menu driven and don't allow free from question answer or exploration.
2. The Chatting application should try to give as accurate answer as possible, if it is unable to answer it should respond that it is not able to answer instead of second guessing the answer.
3. The chatting application should be interactive and respond with answers in a reasonable amount of time.
4. Wherever possible it should be able to explain how it arrived at the answer.
5. If the answer of the query is better served by an existing dashboard it should provide a link to that dashboard.

## Scope
1. Currently we will focus only on English language, but it could be expanded for other high resource Indic languages
2. We will focus only on the data that is captured in the standardised excel sheets, this will ensure that that cross ULB analysis could be correctly done, this may mean that we will skip some additional data uploaded by some of the ULBs
3. Every phase will be having a different scope and will be covered in each one of those sections

## Legal Aspects

The project will use only thsoe cityfinance datasets that are already in public domain.

The code developed in this project will be in Open Source under MIT license and will be made avialable on GitHub repository.

## Cost
The chatign application will internally use a language model, currently the best language models are provided by OpenAI which cost for every query. In this phase we will explore if open source models can be used instead, even though open source models are free to run, they require more powerful machines to run and hence they also have an associated cost.

## Phases
The project will be executed in three phase first phase will be very focussed on technology, whereas the later phases will be focussed on validation with users and deployment.

### Phase I: Technology Validation
This phase is focus on proving that the technology is able to answer questions that are relevant for cityfinance and on their data. This will involve identifying a small set of evaluation questions and their model answers. The software will be compared against this set of model answers.

**Deliverables**: A website with chatting user interface for a limited set of users.

**Duration**: Approximately 2-3 months

**Expectations**: 
 - IIT Bombay Team: Develop the chatting engine for the chatting application.
 - Orgpedia Team: The chat interface for the chatbot and creation of evaluation dataset and metrics. Compare different LLMs and arrive at a pricing estimate for the application.
 - Janaagraha Team: Provide the intial set of standardised excel and weekly time to answer questions on the data and the answers ( 2 hours per week.)

 ### Phase II: User Vaildation
 This phase will test the chatting application with a set of users from different personas and see if it can answer their previously unseen questions. It will also check if it is able to tune the response based on the user personna.

 **Deliverables**: The deliverable will be more optimised chat applications based on the different set of queries and the expected responses on them.

 **Duration**: Approximiately 1 - 1.5 months

 **Expectation**:
 - IIT Bombay Team: Optmize the chatting application based on the different set of queries received from different set of users.
 - Orgpedia Team: An enhanced evaluation set that can be used for model sign off, ensure that it is safe for a public deployment.
 - Janaagraha Team: Create a user-group consisting of people from different user personnas who are going to use this product


 ### Phase III: Deployment and Maintenance
In this phase the chatting application will be deployed on a public facing website where users could come and query the city finance data. We will spell out the exact deliverables and timelines if Phase II is successful.