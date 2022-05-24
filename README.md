# DACON_Samsung_Mol
![20220524_130020](https://user-images.githubusercontent.com/84311270/169952104-38c53c8e-6b19-4a5a-93cb-b7cf20a13819.png)
분자의 3차원 구조 정보를 이용하여 S1-T1 사이의 에너지 갭을 추정할 수 있는 Machine Learning 알고리즘 개발

## Dataset
1. train.csv : 학습 데이터  
uid : 데이터 고유 id  
SMILES : SMILES 화학식  
S1_energy(eV) : 분자의 S1 energy  
T1_energy(eV) : 분자의 T1 energy  

2. train_sdf :t train 분자의 3차원 구조정보  
train_0.sdf  
train_1.sdf  
...

3. dev.csv : 추가 데이터, 학습 사용 가능   
uid : 데이터 고유 id  
SMILES : SMILES 화학식  
S1_energy(eV) : 분자의 S1 energy  
T1_energy(eV) : 분자의 T1 energy  

4. dev_sdf : dev 분자의 3차원 구조정보  
dev_0.sdf  
dev_1.sdf  
...

5. test.csv : 테스트 데이터  
uid : 데이터 고유 id  
SMILES : SMILES 화학식  

6. test_sdf : 분자의 3차원 구조정보  
test_0.sdf  
test_1.sdsf  
...  

7. sample_submissoin.csv : 제출 양식  
uid : 테스트 데이터의 uid  
ST1_GAP(eV) : 분자의 S1 energy - T1 energy 값  
  
## Model
SMILES 분자식을 통해 Chemprop 모델을 사용하여 학습.

## Results
Public Score : 0.14856, Private Score : 0.13684로 최종 43등으로 마무리.
![20220524_130056](https://user-images.githubusercontent.com/84311270/169952483-2b1b06b1-e4fa-45e1-a4f9-47d776b91813.png)

