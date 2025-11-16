# Text-to-Image-to-Video-Model-From-Scratch-Using-GANs
Text-to-video models like OpenAI’s Sora and Stable Video Diffusion are major AI trends in 2024. In this blog, we build a small text-to-video model from scratch: input a prompt, generate a video. We cover the theory, full architecture, and code needed to produce the final output
Since I don’t have a fancy GPU, I’ve coded the small-scale architecture. Here’s a comparison of the time required to train the model on different processors:

| Training Videos | Epochs | CPU | GPU | T4 |
|----------|----------|----------|----------|----------|
| 10K | 30 | more than 3 hr |  1 hr | 1 hr 42 min |
| 30K | 30 | more than 6 hr | 1 hr 30 min | 2 hr 30 min |
| 100K | 30 | - | 3-4 hr | 5-6 hr |

Running on a CPU will obviously take much longer to train the model. If you need to quickly test changes in the code and see results, CPU is not the best choice. I recommend using a T4 GPU from Colab or Kaggle for more efficient and faster training.

Here is the blog link which guides you on how to create Stable Diffusion from scratch: Coding Stable Diffusion from Scratch
