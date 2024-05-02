<h1 align="center">Finetuned LLama3 8b to Generate Java Codes</h1>
<p align="center"><i>This repository contains code for fine-tuning the LLama3 8b model using Alpaca prompts to generate Java codes. The code is based on a Google Colab notebook.</i></p>
<div align="center">
  <a href="https://github.com/Rahul-AkaVector/java-code-generator/stargazers"><img src="https://camo.githubusercontent.com/60270666307048900b8ac19240183d1b18c9dd65c7073cbf36cd5eeab5bfbca8/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f73746172732f736175726162686e61746976652f6372656174652d66726f6e74656e642d726561646d65" alt="Stars Badge"/></a>
<a href="https://github.com/Rahul-AkaVector/java-code-generator/network/members"><img 
src="https://camo.githubusercontent.com/5dd4af823e72b2f3f76ffa17f26348869cb6451ebc4bf5cac8e67ec0c1d02526/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f666f726b732f736175726162686e61746976652f6372656174652d66726f6e74656e642d726561646d65" alt="Forks Badge"/></a>
<a href="https://github.com/Rahul-AkaVector/java-code-generator/pulls"><img src="https://img.shields.io/github/issues-pr/elangosundar/awesome-README-templates" alt="Pull Requests Badge"/></a>
<a href="https://github.com/Rahul-AkaVector/java-code-generator/issues"><img src="https://img.shields.io/github/issues/elangosundar/awesome-README-templates" alt="Issues Badge"/></a>
<a href="https://github.com/Rahul-AkaVector/java-code-generator/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/elangosundar/awesome-README-templates?color=2b9348"></a>
<a href="https://github.com/Rahul-AkaVector/java-code-generator/blob/master/LICENSE"><img src="https://img.shields.io/github/license/elangosundar/awesome-README-templates?color=2b9348" alt="License Badge"/></a>
</div>


## 🚀 Overview

The provided notebook demonstrates how to fine-tune the LLama3 8b model for generating Java codes using Alpaca prompts. It utilizes the `unsloth` library for language model operations and the Hugging Face Transformers library for training and inference tasks.

## 🔗 Links
  - [Google Colab Notebook](https://colab.research.google.com/drive/1FG6MQo3kcc6yNKQj34kxgq7lrZtg0U0l?usp=sharing)
  - [Hugging Face Finetuned Model](https://huggingface.co/rahulAkaVector/java_code_generator_finetuned_model/tree/main)
  
## 🛠️ Usage

### Install necessary packages by executing the following commands:
   ```bash
   !pip install "unsloth[colab-new] @ git+https://github.com/unslothai/unsloth.git"
   !pip install --no-deps "xformers<0.0.26" trl peft accelerate bitsandbytes
   ```
### Training the Model

1. Load the LLama3 8b model with pre-defined settings.
2. Format prompts using Alpaca prompt template and load the dataset.
3. Train the model using the provided dataset and Huggingface TRL's `SFTTrainer`.

### Inference

1. Run inference on the trained model by providing an instruction and input. Leave the output blank for generation.
2. Optionally, use a `TextStreamer` for continuous inference to see the generation token by token.

### Saving and Loading Fine-tuned Models

1. Save the final model with LoRA adapters for inference.
2. Load the saved LoRA adapters for inference if needed.

## 📝 Notes

- Adjust parameters and settings as per your requirements.
- Ensure to replace placeholder file paths with actual paths in the notebook.

##  📚  References

- [Huggingface Transformers Documentation](https://huggingface.co/docs/transformers/index.html)
- [Unsloth GitHub Repository](https://github.com/unslothai/unsloth)


## 🍰 Contribute

Contributions are always welcome! Please create a PR to add Github Profile. Feel free to explore and modify the provided notebook as needed for your Java code generation tasks!

## 🛡️ License

This project is licensed under [MIT](https://opensource.org/licenses/MIT) license.

## 💖 Show your support

Give a ⭐️ if this project helped you!
