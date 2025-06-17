<div align="center">
<h2 align="center">
   <img src="./assets/optimus2.png" style="vertical-align: middle; height: 1em; padding: 0 0.2em;"> <b>Optimus-2: Multimodal Minecraft Agent with Goal-Observation-
     <br />  Action Conditioned Policy
   <br /> <font size=3>CVPR 2025 </font></b> 
</h2>
<div>
<a target="_blank" href="https://scholar.google.com/citations?user=TDBF2UoAAAAJ&hl=en&oi=ao">Zaijing&#160;Li</a><sup>1 2</sup>,
<a target="_blank" href="https://scholar.google.com/citations?user=KO77A2oAAAAJ&hl=en">Yuquan&#160;Xie</a><sup>1</sup>,
<a target="_blank" href="https://scholar.google.com/citations?user=9Vc--XsAAAAJ&hl=en&oi=ao">Rui&#160;Shao</a><sup>1&#9993</sup>,
<a target="_blank" href="https://scholar.google.com/citations?user=Mpg0w3cAAAAJ&hl=en&oi=ao">Gongwei&#160;Chen</a><sup>1</sup>,
<br>
<a target="_blank" href="https://scholar.google.com/citations?hl=en&user=Awsue7sAAAAJ">Dongmei&#160;Jiang</a><sup>2</sup>,
 <a target="_blank" href="https://scholar.google.com/citations?hl=en&user=yywVMhUAAAAJ">Liqiang&#160;Nie</a><sup>1&#9993</sup>
</div>
<sup>1</sup>Harbin Institute of Technology,Shenzhen&#160&#160&#160</span>
<sup>2</sup>Peng Cheng Laboratory, Shenzhen</span>
<br />
<sup>&#9993&#160;</sup>Corresponding author&#160;&#160;</span>
<br/>
<div align="center">
    <a href="https://arxiv.org/abs/2502.19902" target="_blank">
    <img src="https://img.shields.io/badge/Paper-arXiv-deepgreen" alt="Paper arXiv"></a>
    <a href="https://cybertronagent.github.io/Optimus-2.github.io/" target="_blank">
    <img src="https://img.shields.io/badge/Project-Optimus--2-9cf" alt="Project Page"></a>
</div>
</div>



## :new: Updates
- [06/2025] :fire: We released the third generation of Minecraft agent, [Optimus-3](https://arxiv.org/pdf/2506.10357)! [Play with Optimus-3 now!](https://github.com/JiuTian-VL/Optimus-3) We are refactoring Optimus-1 and Optimus-2 to adapt them to the new framework, like Optimus-3.
- [04/2025] :fire: We release the MGOA dataset on [Hugging Face](https://huggingface.co/datasets/MinecraftOptimus/MGOA).
- [03/2025] :fire: [Project page](https://cybertronagent.github.io/Optimus-2.github.io/) released.
- [02/2025] :fire: [Arxiv paper](https://arxiv.org/abs/2502.19902) released.



## :balloon: Optimus-2 Framework
We propose Optimus-2, a novel Minecraft agent that incorporates a Multimodal Large Language Model (MLLM) for high-level planning, alongside a Goal-Observation-Action Conditioned Policy (GOAP) for low-level control. GOAP contains (1) an Action-guided Behavior Encoder that models causal relationships between observations and actions at each timestep, then dynamically interacts with the historical observation-action sequence, consolidating it into fixed-length behavior tokens, and (2) an MLLM that aligns behavior tokens with open-ended language instructions to predict actions auto-regressively.
<img src="./assets/fig2.png" >

## :smile_cat: Evaluation results
We report the `average rewards (AR)` for Atomic Tasks, `average success rate (SR)` for Long-Horizon Tasks and Open-Ended Instruction Tasks.

Table 1: Main Result of GOAP on Atomic Tasks.
<img src="./assets/table1.png" >

Table 2: Main Result of Optimus-2 on Long-Horizon Tasks.
<img src="./assets/table2.png" >

Table 3: Main Result of Optimus-2 on Open-Ended Instruction Tasks.
<img src="./assets/table3.png" >

## :hugs: Citation

If you find this work useful for your research, please kindly cite our paper:

```
@InProceedings{Li_2025_CVPR,
    author    = {Li, Zaijing and Xie, Yuquan and Shao, Rui and Chen, Gongwei and Jiang, Dongmei and Nie, Liqiang},
    title     = {Optimus-2: Multimodal Minecraft Agent with Goal-Observation-Action Conditioned Policy},
    booktitle = {Proceedings of the Computer Vision and Pattern Recognition Conference (CVPR)},
    month     = {June},
    year      = {2025},
    pages     = {9039-9049}
}
```



