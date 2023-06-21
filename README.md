# Robo Advisor for Retirement Plans

This project consists of an AWS Lambda function and an Amazon Lex bot that you can use to get investment portfolio recommendations based on your risk level.

## Step 1: Configure the Initial Robo Advisor
1. Sign in to your AWS Management Console and create a new custom Amazon Lex bot.
   - Bot name: RoboAdvisor
   - Language: English (US)
   - Output voice: Salli
   - Session timeout: 5 minutes
   - Sentiment analysis: No
   - COPPA: No
   - Advanced options: No

2. Add a new intent, named "recommendPortfolio", with sample utterances and four required slots (name, age, investmentAmount, riskLevel).

## Step 2: Build and Test the Robo Advisor
1. Click the "Build" button to build your bot.
2. Test it in the "Test bot" pane. Record a video or create an animated GIF of the working bot.

## Step 3: Enhance the Robo Advisor with an Amazon Lambda Function
1. Create a new Lambda function named "recommendPortfolio" with Python 3.7 as the runtime programming language.
2. In the online code editor, paste the completed `lambda_function.py` (see the Python code below).
3. Test your Lambda function using the provided test events.
4. Integrate your new Lambda function into the bot by selecting it in the “Lambda initialization and validation” and “Fulfillment” sections in the Amazon Lex console.
5. Build your bot, and then test it with both valid and invalid data for the slots. Record a video or create an animated GIF of the working bot.