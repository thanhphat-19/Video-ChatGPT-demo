# Running Video-ChatGPT Demo 
Please follow the instructions below to run the Video-ChatGPT demo on your local GPU machine. 

Note: Our demo requires approximately 18 GB of GPU memory.

### Clone the repository

```shell
cd Video-ChatGPT
export PYTHONPATH="./:$PYTHONPATH"
```

### Install GIT lFS
```shell
git lfs install
```

### Access Token Huggingface to Download The Model

```shell
    huggingface-cli
```


### Download Video-ChatGPT weights

```shell
git clone https://huggingface.co/mmaaz60/LLaVA-7B-Lightening-v1-1
```


### Download LLaVA weights model
```shell
git clone https://huggingface.co/MBZUAI/Video-ChatGPT-7B
```

### Download sample videos

Download the sample videos to test the demo from [this link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/hanoona_bangalath_mbzuai_ac_ae/Ef0AGw50jt1OrclpYYUdTegBzejbvS2-FXBCoM3qPQexTQ?e=TdnRUG)
and place them in `video_chatgpt/demo_sample_videos` directory.

### Run the Demo

```shell
python video_chatgpt/demo/video_demo.py         
--model-name "../../Video-ChatGPT-demo/LLaVA-7B-Lightening-v1-1"         
--projection_path "../../Video-ChatGPT-demo/Video-ChatGPT-7B/video_chatgpt-7B.bin"
```
Follow the instructions on the screen to open the demo dashboard.