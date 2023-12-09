# TEAM_3953

# 專案介紹: 
旨在處理醫療報告中的PHI值及時間正規化，以語言模型 (Language Model)為主要演算法，訓練一個能夠理解和生成自然語言文本的模型，以標註資訊

# 環境需求: 
google colaboratory（免費版）

# 程式碼基本功能：
主要包含以下功能：
1.設置隨機種子： set_torch_seed() 函數設定 PyTorch 中的隨機種子，確保機器學習或深度學習的可重複性。
2.文件和標註資訊處理： read_file() 函數讀取文件內容，process_annotation_file() 函數將標註文件轉換為字典格式。
3.處理醫療報告： process_medical_report() 函數處理醫療報告文本，生成包含標註資訊的序列。
4.並行生成標註的醫療報告： generate_annotated_medical_report_parallel() 函數從標註文件和醫療報告文件中，生成帶有標註資訊的醫療報告，並寫入到 TSV 文件中。
5.資料加載和處理： 使用 load_dataset() 載入資料集，進行預處理。
6.建立模型和訓練： 使用 Transformers 庫建立模型，包括EPOCHS、optimizer及scheduler的調整，並進行訓練。
7.生成醫療報告的預測： 使用訓練好的模型進行預測，生成帶有標註資訊的醫療報告。

# 檔案資料夾說明：
在google drive裡面設立一資料夾名字叫作aicup，裡面除了主要程式檔AICUP2023.ipynb，也包括以下資料夾：

(1) First_Phase_Release：包含主辦方釋出的第一部份訓練集和對應answer檔
(2) Second_Phase_Dataset：包含主辦方釋出的第二部份訓練集和對應answer檔
(3) Validation_Dataset：包含主辦方釋出的驗證集標註檔和對應的answer檔
(4) opendid_test：包含本次比賽的測試檔
(5) train：內含資料處理完的tsv檔
(6) models：儲存訓練模型
最後輸出的answer檔，也會儲存在aicup檔案底下。

![image](https://github.com/coolcoolliang/TEAM_3953/assets/153353877/75afdfc3-43d3-4f18-8fc2-8cffde8f6505)
