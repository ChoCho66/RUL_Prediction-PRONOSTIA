# 實作過程
(1) 存儲資料到 pickle 文件（data_pkz.ipynb）

將學習資料集目錄（Bearing1_1、Bearing1_2、Bearing2_1、Bearing2_2、Bearing3_1、Bearing3_2）的所有文件轉換為單一合併的 pickle(.pkz) 文件（bearing1_1.pkz、bearing1_2.pkz、bearing2_1.pkz、bearing2_2.pkz、bearing3_1.pkz、bearing3_2.pkz），以便於數據存取和更快的數據查詢。

(2) 資料預處理和信號處理（DP_SP.ipynb）

對 1D 信號應用小波變換（CWT），並轉換為標準化的 2D 特徵。

(3) PyTorch 的資料集和 DataLoader（torch_Dataset_DataLoader.ipynb）

使用 PyTorch（或 Torch）的資料集和 DataLoader 來輕鬆存取（查詢、獲取、取得、讀取、檢查）數據，用於機器學習和深度學習模型。解決任何機器學習問題時，許多努力都會投入到資料的準備（預處理）中。PyTorch 提供了許多工具來簡化數據加載（激活），並使代碼更易於閱讀。

DataLoader 在模型訓練過程中提供數據加載的隨機化。

(4) CNN 模型訓練（CNN_Model_Train.ipynb）

使用 PyTorch 框架訓練 CNN 模型進行故障概率預測，並在所有 6 個學習資料集上驗證或評估模型性能。

(5) 將資料打包成序列供 CNN + LSTM 模型使用（CNN+LSTM_Dataset_Preparation.ipynb）

LSTM 需要數據在序列中，因此將原始數據的連續序列打包在一起，並使用 torch Dataset 和 DataLoader 加載。

(6) CNN + LSTM 模型訓練（CNN+LSTM_Model_Train.ipynb）

使用 PyTorch 框架訓練 CNN + LSTM 模型進行故障概率預測，並在所有 6 個學習資料集上驗證或評估模型性能。

(7) 將測試資料存儲到 pickle 文件中（Test_Data_pkz.ipynb）

將測試資料集目錄（Bearing1_3、Bearing1_4、Bearing1_5、Bearing1_6、Bearing1_7、Bearing2_3、Bearing2_4、Bearing2_5、Bearing2_6、Bearing2_7、Bearing3_3）的所有文件轉換為單一合併的 pickle(.pkz) 文件（bearing1_3.pkz、bearing1_4.pkz、bearing1_5.pkz、bearing1_6.pkz、bearing1_7.pkz、bearing2_3.pkz、bearing2_4.pkz、bearing2_5.pkz、bearing2_6.pkz、bearing2_7.pkz、bearing3_3.pkz），以便於數據存取和更快的數據查詢。

(8) 在測試資料上進行資料預處理和信號處理（Test_Dataset_Preparation.ipynb）

對 1D 信號應用小波變換（CWT），並轉換為標準化的 2D 特徵。

(9) 在測試資料上使用 CNN + LSTM 模型（CNN+LSTM_Model_on_Test_data.ipynb）

使用 PyTorch Dataset 和 DataLoader 將 2D 測試資料特徵加載到已訓練的 CNN + LSTM 模型中。
