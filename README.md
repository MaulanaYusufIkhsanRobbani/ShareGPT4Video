# <img src="https://raw.githubusercontent.com/ShareGPT4V/ShareGPT4V-Resources/master/images/share4video_tight.png" style="vertical-align: -10px;" :height="50px" width="50px"> ShareGPT4Video: Improving Video Understanding and Generation with Better Captions

⭐️ **Our series works:** [[**MMStar**](https://mmstar-benchmark.github.io/)]  [[**ShareGPT4V**](https://sharegpt4v.github.io/)]  [[**ShareGPT4Omni**](https://sharegpt4omni.github.io/)]


---

🚀🚀🚀 Official implementation of **ShareGPT4Video: Improving Video Understanding and Generation with Better Captions**.

Here is a video for introducing ShareGPT4Video clearly:

[![video]](https://user-images.githubusercontent.com/56393454/334307144-1b106612-447b-4e35-bb9f-9b904fa3a464.mp4)

- **Authors**: [Lin Chen*](https://lin-chen.site), [Xilin Wei*]() [Jinsong Li*](https://li-jinsong.github.io/), [Xiaoyi Dong](https://scholar.google.com/citations?user=FscToE0AAAAJ&hl=en), [Pan Zhang](https://panzhang0212.github.io/), [Yuhang Zang](https://yuhangzang.github.io/), [Zehui Chen](https://lovesnowbest.site/), [Haodong Duan](https://kennymckormick.github.io/), [Bin Lin](https://scholar.google.com.hk/citations?user=GCOVDKoAAAAJ&hl=en), [Zhenyu Tang](), [Li Yuan](https://yuanli2333.github.io/), [Yu Qiao](https://scholar.google.co.uk/citations?user=gFtI-8QAAAAJ&hl=en), [Dahua Lin](http://dahua.site/), [Feng Zhao📧](https://scholar.google.com/citations?hl=en&user=r6CvuOUAAAAJ), [Jiaqi Wang 📧](https://myownskyw7.github.io/)
- **Institutes**: University of Science and Technology of China; The Chinese University of Hong Kong; Peking University; Shanghai AI Laboratory
- **Resources**: [[Paper](https://arxiv.org/abs/2406.04325v1)] [[Project Page](https://sharegpt4video.github.io/)] [[ShareGPT4Video Dataset](https://huggingface.co/datasets/ShareGPT4Video/ShareGPT4Video)]
- **Models**: [[🤗ShareGPT4Video-8B](https://huggingface.co/Lin-Chen/sharegpt4video-8b)] [[🤗ShareCaptioner-Video](https://huggingface.co/Lin-Chen/ShareCaptioner-Video)]
- **Demo**: [[🤗ShareGPT4Video-8B](https://huggingface.co/spaces/Lin-Chen/ShareGPT4Video-8B)] [[🤗ShareCaptioner-Video](https://huggingface.co/spaces/Lin-Chen/ShareCaptioner-Video)]

## 💡 Highlights

- 🔥 A **large-scale** **highly descriptive** video-text dataset, **40K** GPT4-Vision-generated video captions, around **400K** implicit video split captions.
- 🔥 A **general video captioner for various video durations, resolutions, and aspect ratios**, approaching GPT4-Vision's caption capability, featuring two inference modes targeted for quality and efficiency, separately.
- 🔥 A superior large video-language model **ShareGPT4Video-8B**, lasting **5 hours** on 8xA100 GPUs of training respectively.
- 🔥 **Improving Text-to-Video performance** with high-quality video captions generated by our ShareCaptioner-Video. Thanks to [Open-Sora-Plan](https://github.com/PKU-YuanGroup/Open-Sora-Plan).

## 📜 News

**[2024/6/11]** The web demo and local demo of ShareCaptioner-Video are available now!

**[2024/6/11]** The web demo and local demo of ShareGPT4Video-8B are available now!

**[2024/6/7]** Our paper has been featured as [HuggingFace Daily Papers](https://huggingface.co/papers?date=2024-06-07) and ranked 1st in 6.7.

**[2024/5/27]** The [ShareGPT4Video-8B](https://huggingface.co/Lin-Chen/sharegpt4video-8b) model is released!

**[2024/5/26]** The [ShareGPT4Video dataset](https://huggingface.co/datasets/ShareGPT4Video/ShareGPT4Video) and [project page](https://sharegpt4video.github.io/) are released!

## 👨‍💻 Todo

- [ ] Training and evaluation code for ShareGPT4Video-8B
- [ ] Batch inference code fro ShareCaptioner-Video
- [x] Web demo and local demo of ShareCaptioner-Video
- [x] Web demo and local demo of ShareGPT4Video-8B
- [x] Checkpoints of ShareGPT4Video-8B

## Quick Usage

You can directly use our ShareGPT4Video model for conversation with your own video by the following command:

```
python run.py --model-path Lin-Chen/sharegpt4video-8b --video examples/yoga.mp4 --query Describe this video in detail.
```

Or you can build your local demo for enjoying our ShareGPT4Video-8B with the following command:

```
python app.py
```

You can build your local demo for enjoying our ShareCaptioner-Video with the following command:

```
cd captioner

python app.py
```

## Install

```bash
git clone https://github.com/ShareGPT4Omni/ShareGPT4Video
conda create -n share4video python=3.10 -y
conda activate share4video

cd ShareGPT4Video
pip install --upgrade pip
pip install -e .
pip install -e ".[train]"
pip install flash-attn --no-build-isolation
```

## ✒️ Citation
If you find our work helpful for your research, please consider giving a star ⭐ and citation 📝
```bibtex
@article{chen2024sharegpt4video,
  title={ShareGPT4Video: Improving Video Understanding and Generation with Better Captions},
  author={Chen, Lin and Wei, Xilin and Li, Jinsong and Dong, Xiaoyi and Zhang, Pan and Zang, Yuhang and Chen, Zehui and Duan, Haodong and Lin, Bin and Tang, Zhenyu and others},
  journal={arXiv preprint arXiv:2406.04325},
  year={2024}
}
```

## ❤️ Acknowledgments

- [LLaVA](https://github.com/haotian-liu/LLaVA): the codebase we built upon. Thanks for their wonderful work.
- [Open-Sora-Plan](https://github.com/PKU-YuanGroup/Open-Sora-Plan): an excellent open-source codebase for Sora-like text-to-video implementation. Thanks for their wonderful work.
- [Open-LLaVA-NeXT](https://github.com/xiaoachen98/Open-LLaVA-NeXT): an open-source codebase for re-producing the training procedure of LLaVA-NeXT series.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=ShareGPT4Omni/ShareGPT4Video&type=Date)](https://star-history.com/#ShareGPT4Omni/ShareGPT4Video&Date)
