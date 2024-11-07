# Product-complaint-chatBot

Amazon lex oriented product complaint chatbot using aws

Terminologies:
--->Intent: An intent performs an action in response to natural language user input
--->Utterances: Spoken or typed phrases that invoke your intent
--->Slots: are input data required to fulfill the intent
--->Fulfillment: mechanism for your intent


->Aws console :arrow_right: Amazon Lex->Get started->Create Bot

Step-1: CREATING BOT
1)Bot Name: ComplaintManagement
2)IAM Permissions: Create a role with basic Amazon Lex permissions.
3)Language :English


Step-2: INTENTS & UTTERANCES
1)Intent name: RegisterComplaint
2)Description: This bot helps in registering product complaints
3)Utterances:
Hi
Hello
Hey,I have issues with my product
Hey,I have problem with my product
I want to report a problem with my order
etc...
4)Toggle confirmation prompts to active
5)Toggle   closing responses to active
Save Intent

Step-3: Slot Types
Intent gets fulfilled only when slots are fulfilled, slots are like placeholders for intents
1)1st slot:ProductName
![image](https://github.com/user-attachments/assets/33fdc269-34c9-4430-8a30-e21a58f718af)
2)2nd slot:ProductIssue
![image](https://github.com/user-attachments/assets/d9956516-af3a-4114-96d2-04d3a391e74d)

Step-4: Basic settings
Navigate back to the RegisterComplaint intent
1)Add slot
i)Name 
Data Type: AMAZON.FirstName
Prompts: Hello! May I know your name?

ii)ProductName
Data Type: ProductName
Prompts: Hey (Name), I am Azira bot and I am hapy to assist you today. Please let me know the product you are facing issue with.

iii)ProductIssue
Data Type: ProductIssue
Prompts: I am so sorry to hear that you are facing an issue with (ProductName). Could you please provide me further details so that I can help you further.

iv)CallBackTime
Data Type: AMAZON.Time
Prompts: Our support executive would reach out to you within 24 hours. Could you please let us know your prefered time for the call?

v)PhoneNumber
Data Type: AMAZON.PhoneNumber
Prompts: Please drop your phone number so that our support executive can contact you at (CallBackTime)


Step 5_Confirmation prompts
![image](https://github.com/user-attachments/assets/f2407f76-571b-49fe-b2fb-450ecca0c348)


Step-6: Enhancing user experience by giving advanced options in slots
Select a slot>advanced options>toggle preview>add a card group
give buttons


![image](https://github.com/Vaishnav88sk/product-complaint-chatbot/blob/main/assets/Screenshot%20from%202024-11-07%2020-30-03.png)
![image](https://github.com/Vaishnav88sk/product-complaint-chatbot/blob/main/assets/Screenshot%20from%202024-11-07%2020-30-34.png)
![image](https://github.com/Vaishnav88sk/product-complaint-chatbot/blob/main/assets/Screenshot%20from%202024-11-07%2020-30-26.png)










