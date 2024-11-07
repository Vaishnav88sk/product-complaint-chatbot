# Product-complaint-chatBot

## Amazon lex-oriented product complaint chatbot using AWS.

## Terminologies:
:arrow_right: Intent: An intent performs an action in response to natural language user input\
:arrow_right: Utterances: Spoken or typed phrases that invoke your intent\
:arrow_right: Slots: are input data required to fulfill the intent\
:arrow_right: Fulfillment: mechanism for your intent


:arrow_right: Aws console :arrow_right: Amazon Lex :arrow_right: Get started :arrow_right: Create Bot

## Step-1: CREATING BOT
### 1)Bot Name: ComplaintManagement
### 2)IAM Permissions: Create a role with basic Amazon Lex permissions.
### 3)Language: English


## Step-2: INTENTS & UTTERANCES
###  1)Intent name: RegisterComplaint
###  2)Description: This bot helps in registering product complaints
###  3)Utterances:
####   Hi
####   Hello
####   Hey, I have issues with my product
####   Hey, I have a problem with my product
####   I want to report a problem with my order
####   etc...
###  4)Toggle confirmation prompts to active
###  5)Toggle   closing responses to active
###  Save Intent

## Step-3: Slot Types
Intent gets fulfilled only when slots are fulfilled, slots are like placeholders for intents
### 1)1st slot:ProductName
<img src="https://github.com/user-attachments/assets/33fdc269-34c9-4430-8a30-e21a58f718af" width="700" height="400" />
### 2)2nd slot:ProductIssue
<img src="https://github.com/user-attachments/assets/d9956516-af3a-4114-96d2-04d3a391e74d" width="700" height="400" />

## Step-4: Basic settings
Navigate back to the RegisterComplaint intent
###  Add slot
####   i)Name 
   :arrow_right: **Data Type**: AMAZON.FirstName
   :arrow_right: **Prompts**: Hello! May I know your name?

####   ii)ProductName
   :arrow_right: **Data Type**: ProductName
   :arrow_right: **Prompts**: Hey (Name), I am Azira bot and I am happy to assist you today. Please let me know the product you are facing issue with.

####   iii)ProductIssue
   :arrow_right: **Data Type**: ProductIssue
   :arrow_right: **Prompts**: I am so sorry to hear that you are facing an issue with (ProductName). Could you please provide me with further details so that I can help you further.

####   iv)CallBackTime
   :arrow_right: **Data Type**: AMAZON.Time
   :arrow_right: **Prompts**: Our support executive will reach out to you within 24 hours. Could you please let us know your preferred time for the call?

####   v)PhoneNumber
   :arrow_right: **Data Type**: AMAZON.PhoneNumber
   :arrow_right: **Prompts**: Please drop your phone number so that our support executive can contact you at (CallBackTime)


## Step 5_Confirmation prompts
<img src="https://github.com/user-attachments/assets/f2407f76-571b-49fe-b2fb-450ecca0c348" width="700" height="400" />


## Step-6: Enhancing user experience by giving advanced options in slots
### Select a slot :arrow_right: advanced options :arrow_right: toggle preview :arrow_right: add a card group
### Give Buttons


![image](https://github.com/Vaishnav88sk/product-complaint-chatbot/blob/main/assets/Screenshot%20from%202024-11-07%2020-30-03.png)
![image](https://github.com/Vaishnav88sk/product-complaint-chatbot/blob/main/assets/Screenshot%20from%202024-11-07%2020-30-34.png)
![image](https://github.com/Vaishnav88sk/product-complaint-chatbot/blob/main/assets/Screenshot%20from%202024-11-07%2020-30-26.png)










