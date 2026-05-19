# KorQuAD QA with GPT Data Augmentation

## 프로젝트 개요
GPT-3.5를 활용한 데이터 증강이 한국어 QA 모델 성능에 미치는 영향 분석

## 참고 논문
GPT3Mix: Leveraging Large-scale Language Models for Text Augmentation (Yoo et al., 2021)

## 실험 구성
| 실험 | 학습 데이터 | 결과 |
|------|------------|------|
| Baseline | 원본 3,000개 | Loss: / EM: / F1: |
| Augmented | 원본 + 증강 9,000개 | Loss: / EM: / F1: |

## 모델
- T5: paust/pko-t5-small
- 증강: gpt-3.5-turbo

## 결과
### baseline
![Loss](results/01_baseline_visualization.PNG) <br/>
### augmentation
![EM/F1](results/02_augmentation_visualization.PNG)

## 실험 환경
- Python 3.10
- PyTorch 2.x
- transformers 4.x
