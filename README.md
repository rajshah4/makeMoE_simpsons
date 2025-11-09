# makeMoE Simpsons Edition

<div align="center">
    <img src="images/makemoelogo.png" width="500"/>
</div>

#### A sparse mixture of experts language model, built from scratch—now featuring the Simpsons dataset!

Welcome to **makeMoE**! This project is a playful and educational reimagining of Andrej Karpathy's [makemore](https://github.com/karpathy/makemore), deeply inspired by the Mixture of Experts (MoE) work of [AviSoori1x](https://huggingface.co/blog/AviSoori1x/makemoe-from-scratch). If you're curious about MoE architectures or want to tinker with a modern language model, you're in the right place.

[makeMoE_from_Scratch.ipynb](makeMoE_from_Scratch.ipynb): The main, fully-commented notebook—**start here!**

**What’s new here?**  
This repo extends the original ideas with the Simpsons dataset, richer guidance, and detailed, beginner-friendly comments—especially in the main notebook.

---

### What is makeMoE?

makeMoE is a from-scratch implementation of a sparse mixture of experts (MoE) language model, designed for clarity, hackability, and learning. While it builds on the core concepts of makemore, this version is tailored for the Simpsons dataset and comes with expanded explanations and hands-on guidance, especially in `makeMoE_from_Scratch.ipynb`.

### Highlights

- **Simpsons dataset**: Train and experiment with a fun, real-world dataset.
- **Step-by-step guidance**: The main notebook (`makeMoE_from_Scratch.ipynb`) is packed with comments and explanations to help you understand, modify, and extend the model.
- **Sparse MoE architecture**: Move beyond a single feedforward net to a modern, scalable MoE design.
- **Flexible gating**: Includes both top-k and noisy top-k gating mechanisms.
- **Customizable initialization**: Kaiming He initialization is the default, but you can easily switch to Xavier Glorot or others.
- **Expert Capacity**: Support for expert capacity (see the blog and notebook for details).
- **Seamless experiment tracking**: Integrated with wandb for logging training and generations.

### What stays the same?

- **Pure PyTorch**: No extra dependencies required.
- **makemore DNA**: Retains the original’s causal self-attention, training loop, and inference logic.

### References and Resources

- [HuggingFace Community Blog walkthrough](https://huggingface.co/blog/AviSoori1x/makemoe-from-scratch)
- [Part #2 (Expert Capacity)](https://huggingface.co/blog/AviSoori1x/makemoe2)

- [Outrageously Large Neural Networks: The Sparsely-Gated Mixture-Of-Experts Layer](https://arxiv.org/pdf/1701.06538.pdf)
- [Mixtral of Experts](https://arxiv.org/pdf/2401.04088.pdf)

### Repository Structure

- `makeMoE.py`: Complete PyTorch implementation in a single file.
- [`makeMoE_from_Scratch.ipynb`](makeMoE_from_Scratch.ipynb): The main, fully-commented notebook—**start here!**
- `makeMoE_from_Scratch_with_Expert_Capacity.ipynb`: Builds on the main notebook, adding expert capacity for more efficient training.
- `makeMoE_Concise.ipynb`: A minimal, hackable version for quick experimentation.

Happy hacking, and may your experts be ever sparse and your generations ever witty!
