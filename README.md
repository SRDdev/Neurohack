# NeuroHack
Welcome to NeuroHack, a Machine Learning Hackathon organized by the College of Engineering Pune (COEP). The event is open to students interested in using Machine Learning to solve real-world problems.

## Model
This model is available as a `Keras` model on HuggingFace : [model card](https://huggingface.co/SRDdev/Hin2Hing-Keras_NLP)
```python
from huggingface_hub import from_pretrained_keras

model = from_pretrained_keras("SRDdev/Hin2Hing-Keras_NLP")
```

## Problem Statement
The challenge for this hackathon is to develop a Machine Learning model that can accurately translate English sentences into Hinglish. The dataset provided for training and validation includes English, Hindi, and Hinglish sentences. The test dataset includes only English and Hindi sentences.

## Approach
We used Neural Machine Translation using Transformers approach to solve this problem. As there is a lot of similarities in hindi and Hinglish sentence formation, we convert the input english sentence into hindi & then input it to the model which generates a Hinglish sentence.

## Dataset
The dataset used for training and validation includes English, Hindi, and Hinglish sentences. The test dataset includes only English and Hindi sentences.
- [Dataset](https://www.kaggle.com/competitions/neurohack/data?select=NeuroHack)

## Requirements
To run the code, the following libraries are required:

- TensorFlow
- NumPy
- pandas

## Inference

```python
sentence = "Please can you solve this Problem"
output = decode_sequences(sentence)
print(output)
# output : Kripya aap is problem ka samadhan kar sakte he
```

## Contact
In case of any queries or issues, please contact us at Shreyasrd31@gmail.com
