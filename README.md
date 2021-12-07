# coqui_tts_korea
korea tts using coqui tts


# Train detail
- fastspeech2
  - pretrained with kss data 150000 step, uses [fastspeech2.kss.v2](https://drive.google.com/drive/folders/1G3-AJnEsu2rYXYgo2iGIVJfCqqfbpwMu?usp=sharing)
  - finetuned with half_life data 200000 step

- multiband-melgan
  - pretrained with korea concat data (KSS, Zeroth and Pansori-TEDxKR) 1000000 step
  - finetuned with half_life data 4000000 step
    

# Dataset
- [half_life_dataset](https://bbs.ruliweb.com/news/board/1003/read/1962882)
- [KSS Dataset](https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset)
- [Zeroth Korean](https://github.com/goodatlas/zeroth)
- [Pansori-TEDxKR](https://github.com/yc9701/pansori-tedxkr-corpus)


# Required Environment to run
```python

!git clone https://github.com/TensorSpeech/TensorFlowTTS.git
!cd TensorFlowTTS&&pip install .
!pip install git+https://github.com/repodiac/german_transliterate.git#egg=german_transliterate
!pip install h5py==2.10.0

!conda install cudatoolkit=11.2 -c pytorch -c nvidia
!conda install -c conda-forge cudnn-8.2.1.32  
!pip install tensorflow_gpu==2.6.0

# !conda install cudatoolkit=11.1 -c pytorch -c nvidia -y
# !conda install -c conda-forge cudnn-8.0.5.39 -y
# !pip install tensorflow_gpu==2.4.0

!pip install torchaudio==0.9.0 
!pip install gdown
!sudo apt-get install megatools

```

# Acknowledgement and References 
- [TensorFlowTTS](https://github.com/TensorSpeech/TensorFlowTTS)     
- [Multi-band MelGAN](https://arxiv.org/abs/2005.05106)     
- [FastSpeech 2](https://arxiv.org/abs/2006.04558)
- [speech-japanese-korean-vietnamese](http://www.hieuthi.com/blog/2018/04/22/speech-japanese-korean-vietnamese.html)
- [openslr](http://openslr.org/index.html)     
- [half_life_dataset](https://bbs.ruliweb.com/news/board/1003/read/1962882)
- [KSS Dataset](https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset)
- [Zeroth Korean](https://github.com/goodatlas/zeroth)
- [Pansori-TEDxKR](https://github.com/yc9701/pansori-tedxkr-corpus)
- [Fine-Tuning with a small dataset](https://github.com/TensorSpeech/TensorFlowTTS/issues/296)
- [Siri를 아이유 목소리로 바꾸기](https://blog.crux.cx/iu-siri-1/)     
- [인공지능 deep voice를 이용한 TTS(음성합성) 구현하기 _ 손석희 앵커](http://melonicedlatte.com/machinelearning/2018/07/02/215933.html)     
- [SCE-TTS: 내 목소리로 TTS 만들기](https://gist.github.com/yunho0130/a97db3296314cd7076d8436238fa113a)  
- [TensorflowTTS 한국어 예제 써보기](https://enchiridion.tistory.com/69)
- [huggingface_fastspeech2_kss](https://huggingface.co/tensorspeech/tts-fastspeech2-kss-ko)
- [huggingface_TensorFlowTTS](https://huggingface.co/spaces/akhaliq/TensorFlowTTS)
