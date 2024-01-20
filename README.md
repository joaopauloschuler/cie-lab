# cie-lab
Source code for the paper "Enhancing Convolutional Neural Networks with Achromatic and Chromatic Pathways".

Results from the simple architecture:
|Branches|Color space|1st layer filters|1st layer weights|Flops|Val. acc.|Label|
|--------|-----------|-----------------|-----------------|-----|---------|-----|
|1|GRAY|64 (1ch)|1600|2.8M|81.0\% | JP12A01 |
|1|RGB|64 (3ch)|4800|8.5M|84.4\% | JP12A07 |
|1|HSV|64 (3ch)|4800|8.5M|83.7\% | JP12A09 |
|1|HSL|64 (3ch)|4800|8.5M|82.5\% | JP12A10 |
|1|LAB|64 (3ch)|4800|8.5M|84.7\% | JP12A08 |
|2|LAB|3(1ch)+61(2ch)|3125|5.5M (123k+5.4M)|79.3\% | JP12B12 |
|2|LAB|11(1ch)+53(2ch)|2925|5.2M (484k+4.7M)|84.0\%| JP12B09 |
|2|LAB|22(1ch)+42(2ch)|2650|4.7M (1.0M+3.7M)|84.1\%| JP12B03 |
|2|LAB|32(1ch)+32(2ch)|2400|4.3M (1.4M+2.9M)|84.7\%| JP12B08 |
|2|LAB|42(1ch)+22(2ch)|2150|3.9M (1.9M+2.0M)|84.8\%| JP12B04 |
|2|LAB|53(1ch)+11(2ch)|1875|3.3M (2.3M+1.0M)|84.1\%| JP12B05|
|2|LAB|61(1ch)+3(2ch)|1675|3.0M (2.7M+267k)|83.1\%| JP12B97 |


Results with DenseNet-BC L40
|Branches|Color space|1st layer filters|1st layer weights|Flops|Val. acc.|Label|
|--------|-----------|-----------------|-----------------|-----|---------|-----|
|1|RGB|24(3ch)|176K|144M|92.0\%| JP21P02 |
|2|LAB|16(1ch)+8(2ch)|150K|97M|91.9\%| JP21P03 |

