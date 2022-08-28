# bert-multilingual-chatbot
A BERT-based chatbot that can process multilingual conversation

## Troubleshooting
```
2022-08-28 16:16:08.696094: W external/org_tensorflow/tensorflow/core/framework/cpu_allocator_impl.cc:80] Allocation of 367248384 exceeds 10% of free system memory.
2022-08-28 16:16:08.696945: W external/org_tensorflow/tensorflow/core/framework/cpu_allocator_impl.cc:80] Allocation of 367248384 exceeds 10% of free system memory.
2022-08-28 16:16:08.697294: W external/org_tensorflow/tensorflow/core/framework/cpu_allocator_impl.cc:80] Allocation of 367248384 exceeds 10% of free system memory.
```
### solution
1. reduce batch size
