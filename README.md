# Performance Record

## Conformer Result

* Feature info: using fbank feature, dither, cmvn, online speed perturb
* Training info: lr 0.002, batch size 18, 4 gpu, acc_grad 4, 240 epochs, dither 0.1
* Decoding info: ctc_weight 0.5, average_num 20
* Git hash: 919f07c4887ac500168ba84b39b535fd8e58918a

| decoding mode             | CER   |
|---------------------------|-------|
| attention decoder         | 5.18  |
| ctc greedy search         | 4.94  |
| ctc prefix beam search    | 4.94  |
| attention rescoring       | 4.61  |
| LM + attention rescoring  | 4.36  |

