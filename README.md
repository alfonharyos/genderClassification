# genderClassification
Gambar Aplikasi Gender Classification

![image](https://github.com/eyeshieldbat/GenderClassification/assets/109057552/09b6a34d-da15-4728-9f4e-d9761c7af62d)

# Gender Classification (Resnet)

Repository ini dibuat dalam rangka implementasi model deep learning dalam melakukan klasifikasi gender dengan menggunakan dataset dari CelebA. Model deep learning yang digunakan yakni :
  - Resnet : Resnet18, Resnet34, Resnet50 menggunakan Pytorch
  - Dataset : 70:30, 80:20, 90:10

## Parameter uji coba :
1. Learning rate : 0.0001
2. Loss function : CrossEntropyLoss
3. Optimizer : Adam
4. Batch size : 64
5. Epoch : 10

## implementasi :
  - menguji model ratio dataset dengan model resnet18
  - ratio dataset terbaik di uji kembali dengan resnet34 dan resnet50

## Tabel Model
| No | Model | Dataset ratio | Train Acc | Train Loss | Train f1-score | Test Acc | Test Loss | Test f1-score |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Resnet18 | 70:30 | 0.9529 | 0.0018 | 0.9529 | 0.9780 | 0.0011 | 0.9605 |
| 2 | Resnet18 | 80:20 | 0.9596 | 0.0016 | 0.9596 | 0.9710 | 0.0013 | 0.9619 | 
| 3 | Resnet18 | 90:10 | 0.9583 | 0.0016 | 0.9583 | 0.9710 | 0.0015 | 0.9607 | 
| 4 | Resnet34 | 80:20 | 0.9608 | 0.0015 | 0.9607 | 0.9770 | 0.0011 | 0.9640 | 
| 5 | Resnet50 | 80:20 | 0.9608 | 0.0015 | 0.9607 | 0.9780 | 0.0011 | 0.9642 | 

*model deployment pada streamlit menggunakan model resnet34[80:20]* ***model size <100MB***

## Dependencies
requires **Python 3.10.11**
Basic Libraries: [NumPy](http://www.numpy.org/), [Matplotlib](http://www.matplotlib.org/), [Pandas](http://www.pandas.pydata.org)
Domain-specific Libraries: [Pillow](http://www.python-pillow.org/), [scikit-learn](scikit-learn.org)
Deep-learning Frameworks: [PyTorch](pytorch.org)
web-app Frameworks: [Streamlit](streamlit.io)



