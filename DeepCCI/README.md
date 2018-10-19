## [DeepCCI: End-to-end Deep Learning for Chemical-Chemical Interaction Prediction](https://arxiv.org/pdf/1704.08432.pdf)

CCI(Chemical-Chemical interaction)는 후모 물질(Drug), 독성과 치료적 기능 등을 예측에 핵심이 됩니다.
DeepCCI는 End-to-end Deep learniing기법을 CCI에 적용한 것이고, 
hidden Feature는 chemical 구조를 문자열로 표현해주는 SMILES(simplied molecular input line entry system)에서 가져옵니다. 
7가지 비교 항목을 기준으로 기존 machine learning 기법보다 모두 좋은 결과를 나타냈습니다. 

* Introduction

  Interaction은 두개의 개체 사이에서 유사한 기능 또는 대사 경로에서 발생하는 것입니다.

      Protein- Protein
      Compoundprotein,
      miRNA - mRNA
      Chemimcal- Chmical

  CCI를 컴퓨터연산을 적용하기위해 선행되는 것은 다음과 같습니다. 

      서로 상호작용하는 Chemical들로 조합했을 때 치료효과를 예측하는 화합물 상승작용(synergism)
      서로 상호작용하는 Chemical들의 독성을 공유할 가능성이 더 크다는 가정에 근거한 독성예측
      상용화되어 나온 약품과 가장 가깝고 Graphic 측면에 가장 유사한 화학물질 연결하여 제안하는 표적약물 발견연구
      서로 상로작용하는 Chemical들은 동일한 대사경로에 참여한다는 가정하에 생물학적 기능을 확인하는 새로운 연구


  CCI는 기존 학계에서 다양한 연구방법에서 사용하고 있습니다. 
  DeepCCI는  CCI에 대한 학습기반으로 하기에는 어려움이 있어서, 학습기반으로 CCI 예측하는 방법을 채택했습니다.  

  기존 Chemical(Drug)분석은 feature engineering과 predictve activity 두 단계로 나눌 수 있습니다. 

      Feature: Descriptor, ngerprints or molecular representations
      
  * Feature engineering
  
    1. Chemical들로 부터 informative features을 추출
    
        simple counts: atoms, rings and bonds
        topological properties: atom pairs, shapes and conectivites

    2. 추출된 Feature들을 기반으로 후속 분석
    
    Chemical들의 필수 특성을 확인하기위해 5000 개 이상의 다양한 기능이 확인되었습니다.
      
        ex) PubChem, MACCS and CDK ngerprint


  * Predictive activity 
  
    추출된 특징들의 ADMET와 같은 생물학적 활동들과의 관계를 밝히는 단계입니다.
      
        A: Absoption
        D: Distribution
        M: Metabolism
        E: Excretion
        T: Toxicity

    Deep Learning을 이용한 약물분석은 3가지로 분류 할 수 있습니다.
    
    1. Deep Classifier
    
    2. Deep Generator
    
    3. Ent-to-end deep learning
    
    이중에서 DeepCCI는 end-to-end모델을 기반으로 진행했습니다.
    
    
    
    

