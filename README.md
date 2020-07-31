# UniLM
**预训练的自然语言理解（NLU）和生成（NLG）任务模型**

The family of UniLM:
> [**UniLM**](https://github.com/microsoft/unilm/tree/master/unilm): **用于语言理解和生成的统一预训练**

>  [**InfoXLM**](https://github.com/microsoft/unilm/tree/master/infoxlm) (```new```): **多语言/跨语言预训练模型理解与产生**

>  [**MiniLM**](https://github.com/microsoft/unilm/tree/master/minilm): **用于语言理解和生成的小型预训练模型**

>[**LayoutLM**](https://github.com/microsoft/unilm/tree/master/layoutlm): **用于文档理解的多模式（文本+布局/格式+图像）预训练**（例如扫描的文档，PDF等）** (e.g. scanned documents, PDF, etc.)

>  [**s2s-ft**](https://github.com/microsoft/unilm/tree/master/s2s-ft): **序列到序列微调工具包**

## News
- July 16, 2020: [**InfoXLM** (Multilingual UniLM)](https://github.com/microsoft/unilm/tree/master/infoxlm) [arXiv](https://arxiv.org/pdf/2007.07834.pdf)
- June, 2020 (```NEW```): [LayoutLM](https://github.com/microsoft/unilm/tree/master/layoutlm) was accepted by KDD 2020, and [UniLMv2](https://github.com/microsoft/unilm/tree/master/unilm) was accepted by ICML 2020.
- April 5, 2020: [**Multilingual MiniLM**](https://github.com/microsoft/unilm/tree/master/minilm) released!
- September, 2019: [UniLMv1](https://github.com/microsoft/unilm/tree/master/unilm-v1) was accepted by NeurIPS 2019.

## Release

**\*\*\*\*\* ```New February, 2020```: [UniLM v2](https://github.com/microsoft/unilm/tree/master/unilm) | [MiniLM v1](https://github.com/microsoft/unilm/tree/master/minilm) | [LayoutLM v1](https://github.com/microsoft/unilm/tree/master/layoutlm) | [s2s-ft v1](https://github.com/microsoft/unilm/tree/master/s2s-ft) release \*\*\*\*\***

- [x] [**LayoutLM 1.0**](https://github.com/microsoft/unilm/tree/master/layoutlm) (February 18, 2020): 用于文档（图像）理解的预训练模型（例如收据，表格等）. 它在几个下游任务中实现了新的SOTA结果，包括表单理解（FUNSD数据集从70.72到79.27），收据理解(the [ICDAR 2019 SROIE leaderboard](https://rrc.cvc.uab.es/?ch=13&com=evaluation&task=3) from 94.02 to 95.24) and 和文档图像分类 (the RVL-CDIP dataset from 93.07 to 94.42). "[LayoutLM: Pre-training of Text and Layout for Document Image Understanding](https://arxiv.org/abs/1912.13318) ```KDD 2020```"
- [x] [**s2s-ft 1.0**](https://github.com/microsoft/unilm/tree/master/s2s-ft) (February 26, 2020): 微调的PyTorch 的transformer模型，用于序列到序列的语言生成. "[s2s-ft: Fine-Tuning Pre-Trained Transformers for Sequence-to-Sequence Learning](#)"
- [x] [**MiniLM 1.0**](https://github.com/microsoft/unilm/tree/master/minilm) (February 26, 2020): 深度 self-attention 提炼 is all you need (for task-agnostic knowledge distillation of pre-trained Transformers). MiniLM (12-layer, 384-hidden) 实现了 2.7x 加速对比BERT-base (12-layer, 768-hidden) 不仅在NLU任务上，也包括NLG任务. 很小的 MiniLM (6-layer, 384-hidden) 获得 5.3x 加速产生很好的结果. "[MiniLM: Deep Self-Attention Distillation for Task-Agnostic Compression of Pre-Trained Transformers](https://arxiv.org/abs/2002.10957)"
- [x] [**UniLM 2.0**](https://github.com/microsoft/unilm/tree/master/unilm) (February 28, 2020): **unified pre-training** of bi-directional LM (via autoencoding) and sequence-to-sequence LM (via partially autoregressive) w/ **Pseudo-Masked Language Model** for language understanding and generation. UniLM v2 在广泛的自然语言理解和生成任务中实现了新的SOTA. "[UniLMv2: Pseudo-Masked Language Models for Unified Language Model Pre-Training](https://arxiv.org/abs/2002.12804) ```ICML 2020```"



**\*\*\*\*\* October 1st, 2019: UniLM v1 release \*\*\*\*\***

- [x] [**UniLM v1**](https://github.com/microsoft/unilm/tree/master/unilm-v1) (September 30, 2019): 预训练模型和代码 ```NeurIPS 2019``` 论文是 "[Unified Language Model Pre-training for Natural Language Understanding and Generation](https://arxiv.org/abs/1905.03197)". UniLM (v1) achieves the **new SOTA results** in **NLG** (especially **sequence-to-sequence generation**) 任务是包括信息抽取 (the Gigaword and CNN/DM datasets), 问题生成 (the SQuAD QG dataset), etc. 

## License
This project is licensed under the license found in the LICENSE file in the root directory of this source tree.
Portions of the source code are based on the [transformers](https://github.com/huggingface/transformers) project.

[Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct)

### Contact Information

For help or issues using UniLM, please submit a GitHub issue.

For other communications related to UniLM, please contact Li Dong (`lidong1@microsoft.com`), Furu Wei (`fuwei@microsoft.com`).

