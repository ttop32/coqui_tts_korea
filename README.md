# coqui_tts_korea
Korean TTS using coqui TTS (glowtts and multiband melgan) - 한국어 TTS
- [colab](https://colab.research.google.com/drive/1hv37sT7Pq-qKZe9Ihbbp5XZ-A9tsURli?usp=sharing)

# Result
- input text 
  - "신은 우리의 수학 문제에는 관심이 없다. 신은 다만 경험적으로 통합할 뿐이다."
- output  

https://user-images.githubusercontent.com/46513852/145219169-4afa5943-efd1-4792-83c4-44d10db55e3c.mov  

https://user-images.githubusercontent.com/46513852/145219123-9124959d-8705-4123-adc7-e0e9cd8ceac8.mov  









# Train detail
- glowtts
  - trained with kss data 190000 step
  - train ipynb file : coqui_train_glowtts.ipynb
  - google drive link : https://drive.google.com/drive/folders/1quLOabjkAmmw6mFbcCsMqmGxMC4bbbCW
  
- multiband-melgan
  - trained with korea concat data (KSS, Zeroth and Pansori-TEDxKR) 150000 step
  - train ipynb file : coqui_train_mbmelgan.ipynb
  - google drive link : https://drive.google.com/drive/folders/1FOlcOjx47j_ALNw28rZkr62iOWqHY6tE 
    

# Dataset
- [KSS Dataset](https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset)
- [Zeroth Korean](https://github.com/goodatlas/zeroth)
- [Pansori-TEDxKR](https://github.com/yc9701/pansori-tedxkr-corpus)


# Required Environment to run
```python

!pip install TTS
!pip install jamo
!pip install torchaudio==0.9.0
!pip install gdown
!conda install -c conda-forge kaggle -y
!pip install librosa

```

# Acknowledgement and References 
- [coqui tts](https://github.com/coqui-ai/TTS)
- [TensorFlowTTS](https://github.com/TensorSpeech/TensorFlowTTS)    
- [glow tts](https://arxiv.org/abs/2005.11129) 
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
- [huggingface_fastspeech2_kss](https://huggingface.co/tensorspeech/tts-fastspeech2-kss-ko)
- [huggingface_TensorFlowTTS](https://huggingface.co/spaces/akhaliq/TensorFlowTTS)
- [jamo](https://github.com/JDongian/python-jamo)
- [korean.py](https://github.com/TensorSpeech/TensorFlowTTS/blob/master/tensorflow_tts/utils/korean.py)
- [freeconvert](https://www.freeconvert.com/wav-to-mov)











