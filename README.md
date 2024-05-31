# 🎥 Animate Diff Experiment for Advertisement GIFs

Welcome to the **Animate Diff for Advertisement GIFs** repository! This project uses a combination of OpenAI's GPT and the Animate Diff model to create promotional GIFs from text descriptions. 📝✨

## 🚀 Features

- **Text-to-Video Generation**: Generate captivating GIFs from product descriptions.
- **OpenAI GPT **: Uses GPT to create compelling scripts and prompts.
- **LoRA Weights**: Incorporate specialized LoRA weights for GIF generation of specific brands and personalities.

Experiments with Animate diff and LoRA weights
4. **View the results**
   The generated GIFs will be saved in the `output` folder.

## 📈 Experiments and Results

Here are the results of the experiments conducted using various LoRA weights:

### 🥤 Coca-Cola Ad GIFs

| Generated GIFs |
|---|
| ![Coca-Cola GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/890bbf16-3da7-4223-b872-33f5124ea6d9) |
| ![Coca-Cola 2 GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/e6e3c141-35ad-42f0-b939-7fdff6db06ff)


### 💪 Coca-Cola & Dwayne Johnson Ad GIFs

| Generated GIFs |
|---|
| ![Coca-Cola & Dwayne Johnson GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/a411afa1-de9b-4567-9b8e-184e2c4d01b3) |

## 🧠 How It Works

1. **Script and Prompt Generation** 🎭
    - The first step involves using OpenAI's GPT endpoint to generate a commercial script and a detailed text prompt.
    - Example prompt: `"The Rock takes a Coca-Cola bottle and poses with a satisfactory smile, 8k, 4k, UHD, highly detailed"`
2. **Editing prompt** ✂️
    - The next step involves editing the prompt with LoRA weights specific keywords like "th3rock", "kekokelev2" etc (the keyword used while dream-booth fine-tuning)

3. **GIF Creation** 🎞️
    - The generated prompt is then fed into the Animate Diff model, which uses LoRA weights to adapt and produce the corresponding GIF.

4. **Evaluation** 🔍
    - Each generated GIF should be manually evaluated for its quality, with adjustments made to the script (scale of each LoRA weight) and prompt as needed.

## Future Work 📝
  **Improving results for multiple LoRA**
    - There are many techniques for combining LoRAs like Ties and Dare, and I will try to explore them
  **Generating Longer Video sequence**
    - There are some techniques like applying sliding-window to generate longer sequences, I will try to look into this.

## 🤔 FAQs

**Q: Can I use this for any product?**

Absolutely! Just tweak the product name and description in the text prompt, add its corresponding LoRA weights and the model will generate a customized GIF for you.

**Q: How do I add new LoRA weights?**

You can train new LoRA weights for specific objects or you can use sites like [Civitai](https://civitai.com/) where you can find many pre-trained LoRA weights for different objects and styles

## 📫 Contributions

We welcome contributions! Please open an issue or submit a pull request if you have any suggestions or improvements.

## 🙏 Acknowledgements

- OpenAI for GPT
- The developers of the Animate Diff model
- The Civitai community for LoRA weights
- [Coca-Cola LoRA weights](https://civitai.com/models/215825/norfleet-coke-commercials)
- [Dwyane Johnson LoRA weights](https://civitai.com/models/22345/dwayne-the-rock-johnsonlora)

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Thank you for your interest! We hope you enjoy using our animated advertisement GIF generator. 🎉

![Star the Repo](https://img.shields.io/github/stars/abhijitpal1247/animatediff_exp?style=social)

Feel free to reach out if you have any questions or need support. Happy GIF-making! 🚀

