# EmoVits2
Built on [p0p4k/vits2_python](https://github.com/p0p4k/vits2_pytorch), this version adds Mellotron's GST to the Architecture.

---
# TODO list
- [ ] Models
- [ ] Better Inference notebook
- [ ] Better Training notebook
---

# Installation
requieres python >=3.10
1. Clone the repo and cd into it
```
git clone https://github.com/TheDevloper2023/emo-vits2.git
```
```
cd emo-vits2
```
2. deps
   i. You may need to install espeak first
```
pip install -r requirements.txt
```
3. Download Dataset
5. Build Monotonic Alignment Search and run preprocessing if you use your own datasets.
```
# Cython-version Monotonoic Alignment Search
cd monotonic_align
python setup.py build_ext --inplace

# Preprocessing (g2p) for your own datasets. Preprocessed phonemes for LJ Speech and VCTK have been already provided.
# python preprocess.py --text_index 1 --filelists filelists/ljs_audio_text_train_filelist.txt filelists/ljs_audio_text_val_filelist.txt filelists/ljs_audio_text_test_filelist.txt 
# python preprocess.py --text_index 2 --filelists filelists/vctk_audio_sid_text_train_filelist.txt filelists/vctk_audio_sid_text_val_filelist.txt filelists/vctk_audio_sid_text_test_filelist.txt
```
