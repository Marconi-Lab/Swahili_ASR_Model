# Swahili ASR Model Documentation.
---

### `Introduction`

Despite the existence of more than 7000 languages in the world, a small group of just 10 languages dominate the majority of internet usage, accounting for over 70% of global internet users [ according to Statista](https://www.statista.com/statistics/262946/share-of-the-most-common-languages-on-the-internet/) one of the leading providers of market and consumer data in the world.

 This leaves a significant challenge for the development of conversational AI tools for the remaining over 6900 languages, which collectively account for less than 30% of internet usage and are considered low-resource languages.

  Africa is home to more than 2000 languages, a third of the world's spoken language [according to The African Language Program at Harvard](https://alp.fas.harvard.edu/introduction-african-languages#:~:text=With%20anywhere%20between%201000%20and,more%20than%20one%20million%20speakers.). 
  
  This means that individuals in these countries may be even less likely to have access to accurate and relevant healthcare information online.

`Objective of this project`

 This project aims to develop a Kiswahili ASR (Automatic Speech Recognition) model to contribute in solving patient-doctor consultations (conversations) documentation.


 ---

 ### `Why it matters`

 1. Africa has [the highest burden of disease according to a report in 2019](https://ourworldindata.org/grapher/dalys-rate-from-all-causes).

 2. Most of the healthcare system in Africa is often overwhelmed and underfunded. 
 

 Conversational AI tools can be used for tasks such as:
 -  Symptom checking
 -  Disease diagnosis
 - Treatment recommendations
 - Robust documentation
 
 
 The negative health outcomes of a lack of representation of all languages in the digital space include:
 - A lack of accurate diagnosis
 - Inadequate treatment 
 - Missing out on important medical information
 

 
---

 ### `Data we used to fine-tune the ASR`

 We used an open source swahili dataset from  [Common Voice website](https://commonvoice.mozilla.org/en/datasets) that is available on [hugging face dataset hub](https://huggingface.co/datasets/mozilla-foundation/common_voice_11_0)

 
 ---
 ### `Fine-tuned Model`


 We hosted the model on [Hugging Face Hub](https://huggingface.co/AntonyG/fine-tune-wav2vec2-large-xls-r-1b-sw). You can upload a swahili clip from your files, or record from the browser to get a transcription. *(You may experience some errors in the transcription. We are working to make the model smarter)*


 ---
 ### `Documentation`

1. Notebooks on this repo:
- [Audio pre-processing notebook](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/Audio%20reprocessing%20pipeline.ipynb) and [EDA](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/EDA.ipynb) are series of functions for converting a raw audio to MFCCs.

- [Fine_tuning_(a_pretrained_model)_for_Swahili_ASR](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/Fine_tuning_(a_pretrained_model)_for_Swahili_ASR.ipynb) Pre-processing the data from hugging face.

- [Fine_tuning_XLS_R_Wav2Vec2_with_Swahili_corpus_v1](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/Fine_tuning_XLS_R_Wav2Vec2_with_Swahili_corpus_v1.ipynb) is the initial attempt to train on Google colab, but unsuccessful due to limited computing resources.

- [Fine_tuning_XLS-R with swahili corpus](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/Fine_tuning_XLS_R_Wav2Vec2_with_Swahili_corpus.ipynb) is version 1 of fine-tuning and storing the checkpoints on drive.

- [Fine_tuning_XLS-R with swahili corpus](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/Fine_tuning_XLS_R_Wav2Vec2_with_Swahili_corpus_v2.ipynb) is version 2 of fine-tuning and pushed our model checkpoints to Hugging Face Hub.

- [Real_Time_Speech_Recognition_on_Gradio](https://github.com/Marconi-Lab/Swahili_ASR_Model/blob/main/Real_Time_Speech_Recognition_on_Gradio.ipynb) is version 1 attempt to host our model on gradio.

2.  write-ups that accompany this work:
 - A narrative on [literature review](https://medium.com/@gitau_am/on-literature-review-asr-models-219fb2afcf37)

- A second narrative on [data preparation](https://medium.com/@gitau_am/from-raw-data-to-accurate-speech-recognition-asr-my-journey-of-data-preparation-df3a1b0dee3a)

- A third narrative on [model development](https://medium.com/@gitau_am/exploring-asr-model-development-fine-tuning-xls-r-wav2vec2-model-with-swahili-data-b95134d116b8)

- The overall [technical report](https://drive.google.com/file/d/1mMf7kf4hrU6nJT8GOcgznWIHwMtdYrGm/view?usp=sharing)


				

