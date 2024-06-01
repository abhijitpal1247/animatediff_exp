# 🎥 Animate Diff Experiment for Advertisement GIFs

Welcome to the **Animate Diff for Advertisement GIFs** repository! This project uses a combination of OpenAI's GPT and the Animate Diff model to create promotional GIFs from text descriptions. 📝✨

## 🚀 Features

- **Text-to-Video Generation**: Generate captivating GIFs from product descriptions.
- **OpenAI GPT **: Uses GPT to create compelling scripts and prompts.
- **LoRA Weights**: Incorporate specialized LoRA weights for GIF generation of specific brands and personalities.

## 📈 Experiments and Results

Here are the results of the experiments conducted using various LoRA weights:

### 🥤 Coca-Cola Ad GIFs

| Generated GIFs with stable diffusion v1.5 (base-model), AnimateLCM (motion adapter) and tilt-up LoRA| Generated GIFs with epicRealism (base-model), AnimateDiff-Lightning (motion adapter) and zoom-in LoRA|
|---|---|
| ![Coca-Cola GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/890bbf16-3da7-4223-b872-33f5124ea6d9) |![Coca-Cola alt GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/6cd6c2a4-e0c8-40b7-afe8-d3a496d50a65)|
| ![Coca-Cola 2 GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/8021b5f8-afd4-42ad-b73a-8fa9d43b2eb7) |![Coca-Cola alt 2 GIF](https://github.com/abhijitpal1247/animatediff_exp/assets/69110711/54e88515-3c50-4f25-9179-80b8f1455a83)



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
    - The edited prompt is then fed into the Animate Diff model, which uses LoRA weights to adapt and produce the corresponding GIF.

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

Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.

## 🙏 Acknowledgements

- OpenAI for GPT
- The developers of the Animate Diff model
- The Civitai community for LoRA weights
- [Coca-Cola LoRA weights](https://civitai.com/models/215825/norfleet-coke-commercials)
- [Dwyane Johnson LoRA weights](https://civitai.com/models/22345/dwayne-the-rock-johnsonlora)

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Thank you for your interest! I hope you enjoy using the animated advertisement GIF generator. 🎉

![Star the Repo](https://img.shields.io/github/stars/abhijitpal1247/animatediff_exp?style=social)

Feel free to reach out if you have any questions or need support. Happy GIF-making! 🚀

