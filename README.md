# power-platform-chatGPT
 Samples for using ChatGPT with the Power Platform

## PVA to OpenAI

### Deploying the sample

Prerequisites:

- Provision Azure OpenAI service with API Key
  - Deploy the *gpt-35-turbo* model
- Gain Environment Maker access to a Power Platform environment
  - Ensure HTTPS connector is not blocked by DLP rules

Steps:

1. Download the latest PvaToOpenAisolution file from the [Solution File History](/solution-file-history/) folder (or build the solution from the [source](/src/PVAtoOpenAI/) folder)
2. Deploy the solution to a Development environment
3. Publish the solution
4. In the *Help from ChatGPT with Chat History* cloud flow, edit the following placeholder values with your specific values through the **Azure OpenAI Studio**:
   1. ENDPOINT - update to use the endpoint for your Azure OpenAI service
   2. DEPLOYMENT - update to use the name of the deployment of your *gpt-35-turbo* model
   3. APIKEY - update to use one of the keys for the Azure OpenAI service
5. Publish the *Sample-Buster* bot
6. Deploy the bot to a channel (e.g. Teams channel)
