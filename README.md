# bert-multilingual-chatbot
A BERT-based chatbot that can process multilingual conversation

## Sample Outputs
```
response language: en

Query: 你好!
Response: Hi, how is your day? [Intention predicted: GREETINGS]
Query: hello
Response: Hi, how is your day? [Intention predicted: GREETINGS]
Query: 琴日入完tqqq 今日即跌
Response: I lost a lot on stock, sooner I won't even have money to pay the rent cost on AWS EC2... which means you may not reach me later. [Intention predicted: INVESTMENT]
Query: 你辦公時間是甚麼?
Response: As long as the server keeps running, I work 7/24. So just reach me anytime you are free. [Intention predicted: OFFICE_HOUR]
Query: you perform bad
Response: Sorry sorry, I know I am not smart enough. Maybe I will improve in the future with more training data. [Intention predicted: APPRAISAL_BAD]
```
```
response language: zh

Query: 你好!
Response: 你好呀，今日過成點? [Intention predicted: GREETINGS]
Query: hello
Response: 你好呀，今日過成點? [Intention predicted: GREETINGS]
Query: 琴日入完tqqq 今日即跌
Response: 我美股豬咗好多錢吖，我之後可能冇錢去俾AWS EC2 租金添，話唔定你之後會見我唔到啦。 [Intention predicted: INVESTMENT]
Query: 你辦公時間是甚麼?
Response: 只要個server 仲行緊，咁我就會7/24 返工嘅，所以你幾時揾我都得。 [Intention predicted: OFFICE_HOUR]
Query: you perform bad
Response: 真係唔好意思，我知我仲未夠醒目，可能我遲啲有多啲training data會再聰明啲。 [Intention predicted: APPRAISAL_BAD]
```
```
response language: fr

Query: 你好!
Response: Salut, comment est votre journée ? [Intention predicted: GREETINGS]
Query: hello
Response: Salut, comment est votre journée ? [Intention predicted: GREETINGS]
Query: 琴日入完tqqq 今日即跌
Response: J'ai perdu beaucoup de stock, plus tôt je n'aurai même pas d'argent pour payer les frais de retour sur AWS EC2... Ce qui signifie que vous ne pourrez plus me joindre plus tard. [Intention predicted: INVESTMENT]
Query: 你辦公時間是甚麼?
Response: Si le serveur tourne, je travaille 7/24. Alors rendez-moi quand tu es libre. [Intention predicted: OFFICE_HOUR]
Query: you perform bad
Response: Désolé désolé, je sais que je ne suis pas assez intelligent. Peut-être que je m'améliorerai à l'avenir avec plus de données d'entraînement. [Intention predicted: APPRAISAL_BAD]
```

## Hardware Requirements
### Training (based on Google Colab)
1. GPU ram (4.75 GB)

### Running/Prediction
1. GPU ram (2.61 GB in average, 3.8 GB max)

## Troubleshooting
```
2022-08-28 16:16:08.696094: W external/org_tensorflow/tensorflow/core/framework/cpu_allocator_impl.cc:80] Allocation of 367248384 exceeds 10% of free system memory.
2022-08-28 16:16:08.696945: W external/org_tensorflow/tensorflow/core/framework/cpu_allocator_impl.cc:80] Allocation of 367248384 exceeds 10% of free system memory.
2022-08-28 16:16:08.697294: W external/org_tensorflow/tensorflow/core/framework/cpu_allocator_impl.cc:80] Allocation of 367248384 exceeds 10% of free system memory.
```
### solution
1. reduce batch size
