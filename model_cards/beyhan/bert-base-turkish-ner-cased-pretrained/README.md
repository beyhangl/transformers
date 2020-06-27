# Bert-Turkish-NER




## Usage

```python
from transformers import pipeline, AutoModelForTokenClassification, AutoTokenizer
model = AutoModelForTokenClassification.from_pretrained("beyhan/bert-base-turkish-ner-cased-pretrained")
tokenizer = AutoTokenizer.from_pretrained("beyhan/bert-base-turkish-ner-cased-pretrained")
ner=pipeline('ner', model=model, tokenizer=tokenizer)
ner("Tren kalkış saatleri bana uyarsa Ankara'ya trenle gideceğim.")
```

## Results
```
step 4280
runtime 3510.0960245132446
learning_rate 3.2710280373831774e-06

epoch 10.0

loss 0.0009715984738359111
eval_f1 0.9384230856623494
eval_loss 0.08399763153021156
eval_precision 0.9348121321865097
eval_recall 0.9420620437956204
