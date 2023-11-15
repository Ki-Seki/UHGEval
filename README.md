[English](./README.md) | [中文简体](./README.zh_CN.md)

# UHGEval

Benchmarking the Hallucination of Chinese Large Language Models via Unconstrained Generation

Features:
* Safety: Ensuring the security of experimental data is of utmost importance.
* Flexibility: Easily expandable, with all modules replaceable.

## Quick Start

Get started quickly with a 20-line demo program.

* `pip install -r requirements.txt`
* Take `uhgeval/configs/example_config.py` as an example, create `uhgeval/configs/real_config.py` to configure the OpenAI GPT section.
* Run `demo.py`

## Advanced Usage

Run `experiment.py` to delve deeper into the project. You may encounter various issues during the trial run because the project is currently just a demo. For now, you can follow the interpreter's prompts to get the program running smoothly.

## TODOs

<details>
<summary>Click me to show all TODOs</summary>

- [ ] requirements.txt: add version specifications
- [ ] evaluator: add a function, `set_llm()`, to update the llm parameter
- [ ] translate: use English throughout
- [ ] docs: update all documentation
- [ ] llm, metric: enable loading from HuggingFace
- [ ] running.log: enable log saving
- [ ] evaluator: add `XinhuaHallucinationsEvaluator` class between the abstract class and concrete classes

</details>
