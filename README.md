# EEG Data Loading & Spatial Visualization Pipeline using MNE-Python

*A beginner-friendly neuroscience project demonstrating the first stage of an EEG analysis workflow.*

---

# Motivation

### 🇬🇧 English

Coming from a Computer Science background, I thought the importance of understanding how raw biological signals are transformed into structured data, before applying machine learning algorithms.

Rather than jumping into classification models directly, I decided to first build a foundation by learning how EEG recordings are loaded, standardized, and visualized using MNE-Python, one of the most widely adopted open-source libraries in computational neuroscience.

### 🇰🇷 한국어

컴퓨터과학을 공부하면서 머신러닝 모델을 적용하기 이전에, 원시 생체신호가 어떻게 정리되고 분석 가능한 형태로 변환되는지 중요하다고 생각했습니다.

분류(Classification)부터 시작하기보다, 계산신경과학 분야에서 가장 널리 사용되는 MNE-Python을 활용하여 EEG 데이터의 구조와 전처리 과정을 기초부터 학습하기 위해 본 프로젝트를 진행했습니다.

---

# Project Objective

### 🇬🇧 English

This project implements the first stage of a reproducible EEG analysis pipeline.

The objectives:

- Load raw EEG recordings
- Inspect recording metadata
- Standardize EEG channel names
- Apply the international standard_1005 electrode montage
- Visualize electrode locations and raw EEG signals

This project serves as the foundation for future preprocessing and machine learning studies.

### 🇰🇷 한국어

본 프로젝트는 재현 가능한 EEG 분석 파이프라인의 첫 단계를 구현하는 것을 목표로 합니다.

주요 목표:

- 원시 EEG 데이터 불러오기
- 메타데이터 확인
- 채널 이름 표준화
- 국제 표준 standard_1005 전극 좌표계 적용
- EEG 파형 및 전극 위치 시각화

향후 Filtering, ICA, Feature Extraction, Classification 프로젝트의 기반이 되는 단계입니다.

---

# Dataset

### 🇬🇧 English

**PhysioNet EEG Motor Movement/Imagery Dataset**

- Public benchmark dataset
- 64-channel EEG
- Motor execution & motor imagery tasks

https://physionet.org/

### 🇰🇷 한국어

**PhysioNet EEG Motor Movement/Imagery Dataset**

- 국제 공개 EEG 벤치마크 데이터셋
- 64채널 EEG
- 운동 수행 및 운동 상상(Motor Imagery) 실험 데이터

---

# Tech Stack

### 🇬🇧 English

- Python
- MNE-Python
- NumPy
- SciPy
- Matplotlib
- Google Colab

### 🇰🇷 한국어

- Python
- MNE-Python
- NumPy
- SciPy
- Matplotlib
- Google Colab

---

# Repository Structure

```text
eeg-mne-pipeline/

├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│
├── figures/
│   ├── raw_eeg.png
│   └── sensor_topomap.png
│
├── notebooks/
│   └── 01_eeg_loading_visualization.ipynb
│
└── src/
```

---

# Workflow

### 🇬🇧 English

1. Load raw EEG recordings
2. Inspect metadata
3. Standardize channel names
4. Apply standard_1005 montage
5. Visualize electrode positions
6. Inspect raw EEG waveforms

### 🇰🇷 한국어

1. 원시 EEG 데이터 로드
2. 메타데이터 확인
3. 채널 이름 표준화
4. standard_1005 좌표계 적용
5. 전극 위치 시각화
6. 원시 EEG 파형 확인

---

# Results

*(IMAGE)*

### 🇬🇧 English

The EEG channels were successfully mapped onto the international standard_1005 electrode system, providing an anatomically meaningful spatial representation for future signal processing.

### 🇰🇷 한국어

EEG 채널을 국제 표준 standard_1005 전극 좌표계에 성공적으로 매핑하여 향후 신호처리 및 머신러닝 분석을 위한 공간 정보를 구축했습니다.

---

# What I Learned

### 🇬🇧 English

This project helped me understand:

- the structure of EEG recordings
- channel naming conventions
- electrode montages
- why preprocessing is essential before machine learning

It also strengthened my understanding of how computational neuroscience workflows begin from raw biomedical data(rather than from AI models).

### 🇰🇷 한국어

이번 프로젝트를 통해

- EEG 데이터 구조
- 채널 명명 규칙
- 전극 좌표계(Montage)
- 머신러닝 이전 전처리의 중요성

을 이해할 수 있었으며, 계산신경과학 프로젝트는 AI 모델보다 데이터 구조를 이해하는 것부터 시작된다는 점을 배웠습니다.

---

# Limitations

### 🇬🇧 English

This project focuses only on EEG loading and visualization.

The following components would be considered in future projects:

- Filtering
- Artifact Removal (ICA)
- Epoch Extraction
- Feature Engineering
- Motor Imagery Classification
- Deep Learning

### 🇰🇷 한국어

본 프로젝트는 EEG 데이터 로딩과 시각화만을 다룹니다.

향후 프로젝트에서는

- Filtering
- ICA
- Epoching
- Feature Extraction
- Classification
- Deep Learning

구현을 고려할 예정입니다.

---

# How to Run

```bash
pip install -r requirements.txt
```

or simply open the notebook in Google Colab and run all cells.

---

# Acknowledgement

### 🇬🇧 English

This project was independently developed for educational and portfolio purposes using publicly available datasets provided by PhysioNet and the MNE-Python ecosystem.

### 🇰🇷 한국어

본 프로젝트는 PhysioNet과 MNE-Python에서 제공하는 공개 데이터를 활용하여 학습 및 포트폴리오 목적으로 독립적으로 개발되었습니다.