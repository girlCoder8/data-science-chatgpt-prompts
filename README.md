# RentalGPT Dash App 

[Selected as Plotly’s Top ChatGPT & Generative AI Project](https://plotly.com/examples/generative-ai-chatgpt/)

I am presenting the data analysis, data visualization, and Dash application development called "RentalGPT", an interactive, user friendly dashboard that provides services to multiple stakeholders. Using the "Two Sigma Connect: Rental Listing Inquiries" dataset collected from Kaggle, we can do in-depth data analysis, interactive data visualization, and an app that has predictive analytics and virtual assistance.

### Business Understanding & Data Acquisition
The datasets can be found [here]((https://www.kaggle.com/competitions/two-sigma-connect-rental-listing-inquiries/data?select=train.json.zip)).
- `train.json`: the training set.
- `images_sample.zip`: listing images organized by listing_id (a sample of 100 listings)
- `Kaggle-renthop.7z`: listing images organized by listing_id. Total size: 78.5 GB compressed.

**Note**: for this project, we will consider the training dataset as a full-dataset, as our goal is not to beat the competition, but to build a tool for data analysis and usages.

### Data Processing & Feature Engineering
Using various techniques
- Tabular Feature Extraction.
- Sentimental Extraction via HuggingFace's pretrained BERT (benchmark on SST dataset).
- Image Feature Extraction via PyTorch's YOLO.v5.

### ML Modeling
I used Sklearn's SVM, Decision Tree, Random Forest, MLP, KNN.
- **Type 1**: Based on the tabular input of the user (without extracted features from image), can we predict the interest level. 
- **Type 2**: Based on the tabular input of the user and the image, can we predict the interest level.
- **Type 3**: Based on the tabular input of the user (without extracted features from image), can we predict the price. 
- **Type 4**: Based on the tabular input of the user and the image, can we predict the price.

## References
[1] “Two Sigma Connect: Rental Listing Inquiries | Kaggle,” Kaggle.com, 2023. https://www.kaggle.com/competitions/two-sigma-connect-rental-listing-inquiries/data?select=train.json.zip (accessed Nov. 23, 2023).

‌[2] [Huging Chat API](https://github.com/Soulter/hugging-chat-api)

[3] [HugChat Chatbot with Streamlit Blog](https://blog.streamlit.io/how-to-build-an-llm-powered-chatbot-with-streamlit/)

[4] [HugChat Chatbot with Streamlit Code](https://github.com/dataprofessor/hugchat/blob/master/app_v3.py)

[5] [OpenAssistant LLaMA 30B SFT 6](https://huggingface.co/OpenAssistant/oasst-sft-6-llama-30b-xor)

[6] [HuggingChat - New Open Source Alternative to ChatGPT](https://www.youtube.com/watch?v=7QChacb3-00)

[7] [Open Assistant](https://open-assistant.io/)

[8] [Dash with ChatGPT Code](https://github.com/plotly/dash-sample-apps/blob/main/apps/dash-gpt3-chatbot/app.py)

[9] [HugChat API Repository](https://github.com/Soulter/hugging-chat-api/tree/master)