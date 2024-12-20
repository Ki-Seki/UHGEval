# UHGEval

## Information

- **Paper**: UHGEval: Benchmarking the Hallucination of Chinese Large Language Models via Unconstrained Generation
- **Institution**:
  - Renmin University of China
  - Institute for Advanced Algorithms Research, Shanghai
  - State Key Laboratory of Media Convergence Production Technology and Systems
- **Paper Page**: https://iaar-shanghai.github.io/UHGEval/
- **ACL Anthology**: https://aclanthology.org/2024.acl-long.288/
- **arXiv**: https://arxiv.org/abs/2311.15296
- **GitHub**: https://github.com/IAAR-Shanghai/UHGEval
- **Hugging Face**: https://huggingface.co/collections/Ki-Seki/uhgeval-66bc7ebad50f341d156f4073

## Evaluators

| Evaluator                  | Metric                             | Description                                                                          |
| -------------------------- | ---------------------------------- | ------------------------------------------------------------------------------------ |
| `UHGDiscKeywordEvaluator`  | Average Accuracy                   | Given a keyword, the LLM determines whether it contains hallucination.               |
| `UHGDiscSentenceEvaluator` | Average Accuracy                   | Given a sentence, the LLM determines whether it contains hallucination.              |
| `UHGGenerativeEvaluator`   | BLEU-4, ROUGE-L, kwPrec, BertScore | Given a continuation prompt, the LLM generates a continuation.                       |
| `UHGSelectiveEvaluator`    | Accuracy                           | Given hallucinated text and unhallucinated text, the LLM selects the realistic text. |

## Citation

```bibtex
@inproceedings{liang-etal-2024-uhgeval,
    title = "{UHGE}val: Benchmarking the Hallucination of {C}hinese Large Language Models via Unconstrained Generation",
    author = "Liang, Xun  and
      Song, Shichao  and
      Niu, Simin  and
      Li, Zhiyu  and
      Xiong, Feiyu  and
      Tang, Bo  and
      Wang, Yezhaohui  and
      He, Dawei  and
      Peng, Cheng  and
      Wang, Zhonghao  and
      Deng, Haiying",
    editor = "Ku, Lun-Wei  and
      Martins, Andre  and
      Srikumar, Vivek",
    booktitle = "Proceedings of the 62nd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.acl-long.288",
    pages = "5266--5293",
    abstract = "Large language models (LLMs) produce hallucinated text, compromising their practical utility in professional contexts. To assess the reliability of LLMs, numerous initiatives have developed benchmark evaluations for hallucination phenomena. However, they often employ constrained generation techniques to produce the evaluation dataset due to cost and time limitations. For instance, this may involve employing directed hallucination induction or deliberately modifying authentic text to generate hallucinations. These are not congruent with the unrestricted text generation demanded by real-world applications. Furthermore, a well-established Chinese-language dataset dedicated to the evaluation of hallucinations is presently lacking. Consequently, we have developed an Unconstrained Hallucination Generation Evaluation (UHGEval) benchmark, containing hallucinations generated by LLMs with minimal restrictions. Concurrently, we have established a comprehensive benchmark evaluation framework to aid subsequent researchers in undertaking scalable and reproducible experiments. We have also evaluated prominent Chinese LLMs and the GPT series models to derive insights regarding hallucination.",
}
```
