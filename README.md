# POSCO EnC:Acousto-Ultrasonic-Echo-Test

## 제출자료

- [킥오프 회의](pt/kickoff.md)
- [1차 게이트리뷰](pt/gatereview01.md)


## 관련자료

### 진행상황

- [유한요소 해석](doc/fea/FEA_experiment.md)
- [ABAQUS FEA](doc/fea/FEA_ABAQUS.md)
- [고온 탄성계수 시험](doc/experiment/HighTemp_YM_Experiment.md)
- [상온 탄성계수 시험](doc/experiment/RoomTemp_YM_Experiment.md)
- [웨이블릿 변환](doc/waveletTransform.md)
- [온도보정계수](doc/ThermalCorrectionFactor.md)
- [내화물 물성치 DB](data/db/database.md)

### 출장 보고서

- [Hatch 현장 사전탐사 보고서](doc/meeting/preliminaryReport.md)
- [SNNC 1기 전기로 내화물 측정 Test](doc/meeting/SNNC001.md)


### 창원대 산학협력단 담당자

사무원, 박효빈, 213-2813,   [hyobiz@changwon.ac.kr](mailto:hyobiz@changwon.ac.kr)
> 담당자 퇴사 후 변경 진행중

### 회의록

- [2024년 11월 25일 회의록](doc/meeting/meeting_20241125.md)
- [2025년 02월 04일 회의록](doc/meeting/meeting_20250204.md)

## 폴더 관리(GPT)

- [데이터 구조](doc/dataStructure.md)

requirements.txt : 필요 MATLAB 툴박스 목록  
README.md : 프로젝트 개요 및 실행 방법  

>administration/
>>invoice/ : 영수증  

>data/
>>db/ : 물성치DB (CSV 파일 등)  
>>experiment/ : 원본 데이터 (CSV, MAT 파일 등)  
>>>MaterialTest/ : 단위블럭 재료물성 테스트  
>>>FurnaceTest/ : 노 에서 실제 타격한 테스트  
>>>>processed/ : 웨이블릿 변환된 이미지 데이터  
>>>>raw/ : 원본 데이터 (CSV, MAT 파일 등)  

>>profile/ : 내화물 두께 추정DB (CSV 파일 등)  
>> simulated/ : 원본 데이터 (CSV, MAT 파일 등)  

> doc/  
>> meeting/ : 회의록  
>> experiment/ : 실험관련 글  
>> fea/ : 해석관련 글  
<!-- │   ├── features/              % 추출된 피쳐 데이터 (MAT, CSV)  
│   ├── database.mat                % 저장된 데이터베이스 (MATLAB 변수) --> 
> img/ : 

> misc/ : 기타파일 
>> eqip_spec/ : 기기 스펙  
>> schedule/ : 일정  
>> trash/ : 삭제된 항목   

> model/  
>> trained_models/ : 훈련된 모델 저장 (MAT, HDF5)  
>> model_architecture.m : 딥러닝 모델 아키텍처 정의  
>> train_model.m : 모델 학습 및 평가 스크립트  

> pt/  
>> Preliminary/  
>> theme/ 

> src/  
>> thermalCorrectionFactor/ : 물성치DB (CSV 파일 등)  
>>> evaluateTCF.m : 온도보정계수 산정 함수  

> util/  
>> data_loader.m : 데이터 로딩 함수  
>> startup.m : 데이터 및 결과 시각화  
> shutdown.m : 데이터 및 결과 시각화  


wavelet_thickness_estimation/
│-- administration/  
│   ├── invoice/ % 영수증  
│-- data/  
│   ├── db/ : 물성치DB (CSV 파일 등)  
│   ├── experiment/ : 원본 데이터 (CSV, MAT 파일 등)  
│   │   ├── MaterialTest/ : 단위블럭 재료물성 테스트  
│   │   ├── FurnaceTest/ : 노 에서 실제 타격한 테스트  
│   │   │   ├── processed/ : 웨이블릿 변환된 이미지 데이터  
│   │   │   ├── raw/ : 원본 데이터 (CSV, MAT 파일 등)  
│   ├── fea/ : 유한요소해석 DB (CSV, MAT 파일 등)  
│   ├── simulated/ : 원본 데이터 (CSV, MAT 파일 등)  
│-- doc/  
│   ├── meeting/ : 회의록  
│   ├── experiment/ : 실험관련 글  
│   ├── fea/ : 해석관련 글  
│   │   ├── LS-DYNA_backup/ : LS-DYNA FEA 자료 보관 
<!-- │   ├── features/              % 추출된 피쳐 데이터 (MAT, CSV)  
│   ├── database.mat                % 저장된 데이터베이스 (MATLAB 변수) --> 
│-- img/                            
│-- misc/  
│   ├── eqip_spec/ : 기기 스펙  
│   ├── schedule/                      
│   ├── trash/ : 삭제된 항목   
│-- model/  
│   ├── trained_models/ : 훈련된 모델 저장 (MAT, HDF5)  
│   ├── model_architecture.m : 딥러닝 모델 아키텍처 정의  
│   ├── train_model.m : 모델 학습 및 평가 스크립트  
│-- pt/  
│   ├── Preliminary/                  
│   ├── theme/                        
│-- src/  
│   ├── thermalCorrectionFactor/ : 물성치DB (CSV 파일 등)  
│   │   ├── evaluateTCF.m : 온도보정계수 산정 함수  
│-- util/  
│   ├── data_loader.m : 데이터 로딩 함수  
│   ├── startup.m : 데이터 및 결과 시각화  
│   ├── shutdown.m : 데이터 및 결과 시각화  
│-- requirements.txt : 필요 MATLAB 툴박스 목록  
│-- README.md : 프로젝트 개요 및 실행 방법  


