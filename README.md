# Swahili ASR Model Documentation.
---

### `Introduction`

Despite the existence of more than 7000 languages in the world, a small group of just 10 languages dominate the majority of internet usage, accounting for over 70% of global internet users [ according to Statista](https://www.statista.com/statistics/262946/share-of-the-most-common-languages-on-the-internet/) one of the leading providers of market and consumer data in the world.

 This leaves a significant challenge for the development of conversational AI tools for the remaining over 6900 languages, which collectively account for less than 30% of internet usage and are considered low-resource languages.

 ---

 ### `Why does it matter?`

 Lets take an example with the healthcare domain, conversational AI tools can be used for tasks such as:
 -  Symptom checking
 -  Disease diagnosis
 - Treatment recommendations
 - Robust documentation
 
 If these tools are developed primarily for the most widely-used languages such as English, they may not be able to accurately understand or respond to the unique symptoms, diseases, and cultural context of people who use low-resource languages. 
 
 The problems that can result include:
 - A lack of accurate diagnosis
 - Inadequate treatment 
 - Missing out on important medical information
 
 All these results are examples of how a lack of representation of all languages in the digital space can lead to negative health outcomes. 


#### `Why Healthcare?`

 Africa is home to more than 2000 languages, a third of the world's spoken language [according to The African Language Program at Harvard](https://alp.fas.harvard.edu/introduction-african-languages#:~:text=With%20anywhere%20between%201000%20and,more%20than%20one%20million%20speakers.). Africa being an inhabitant of Low-income countries, it has a higher proportion of speakers of low-resource languages, and also have lower levels of internet penetration and access to technology. This means that individuals in these countries may be even less likely to have access to accurate and relevant healthcare information, yet they have [the highest burden of disease according to a report in 2019](https://ourworldindata.org/grapher/dalys-rate-from-all-causes).

 Furthermore, in low-income countries, the healthcare system is often overwhelmed and underfunded, meaning that the healthcare providers are overworked, so the use of conversational AI tools could be a way to help in providing care and information to patients,

 In conclusion, if these tools are not developed to support low-resource languages, it can further exacerbate existing health disparities and negatively impact the health and well-being of individuals in these countries.

 ---

 ### `What are we doing about it?`

 The main objective of this project is to create a robust documentation system for Swahili conversations between healthcare professionals and patients. 
 
 To achieve this, we aim to develop a Kiswahili ASR (Automatic Speech Recognition) model that is specific to the healthcare domain.

---

 ### `Data`

 We are using an open source dataset from common voice that is available on [hugging face platform](https://huggingface.co/datasets/mozilla-foundation/common_voice_11_0)

 We shall load the data into our notebook using the dataset object from hugging face as shown below.

 `from datasets import load_dataset`

`common_voice_train = load_dataset("mozilla-foundation/common_voice_11_0", "sw", split="train")`

 More commonvoice data can be found on [their website](https://commonvoice.mozilla.org/en/datasets).

 ---
 ### `Documentation`

 This subsection contains write-ups that accompany this work.
 1. A narrative on [literature review](https://medium.com/@gitau_am/on-literature-review-asr-models-219fb2afcf37)

2. A second narrative on [data preparation](https://medium.com/@gitau_am/from-raw-data-to-accurate-speech-recognition-asr-my-journey-of-data-preparation-df3a1b0dee3a)

3. A third narrative on [model development](https://medium.com/@gitau_am/exploring-asr-model-development-fine-tuning-xls-r-wav2vec2-model-with-swahili-data-b95134d116b8)

4. The overall [technical report](https://drive.google.com/file/d/1mMf7kf4hrU6nJT8GOcgznWIHwMtdYrGm/view?usp=sharing)


				

