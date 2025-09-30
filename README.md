# AI 學習歷程檔案產生器
一個使用 **Flask** 與 **Google Gemini API** 開發的應用程式，  
能根據使用者輸入的活動內容與上傳的照片，自動生成學習歷程報告並輸出為 **Word 文件 (.docx)**。  
此專案專為台灣使用者設計，適合學生快速整理學習歷程檔案。
## 功能特色
- 上傳多張活動照片
- 輸入活動名稱、簡介、角色、收穫
- 自動生成包含七大段落的完整報告：
  1. 主題說明
  2. 心得反思
  3. 學習歷程檔案內容簡介（100字內）
  4. 檢討或反思
  5. 學習或執行過程（步驟、結果）
  6. 對未來的影響
  7. 學習成果佐證說明
- 一鍵匯出 **Word 檔（.docx）**，含活動照片
## 安裝方式
### 1. 下載專案
```bash
git clone https://github.com/Chuen666666/ai-portfolio-generator.git
cd ai-portfolio-generator
```
### 2. 建立虛擬環境（建議）
可使用 Venv 建立虛擬環境
### 3. 安裝套件
```bash
pip install -r requirements.txt
```
### 4. 設定 API Key
1. 到 [Google Dev](https://ai.google.dev/) 取得 Gemini API
2. 將檔案 `config.example.ini` 改名為 `config.ini`
3. 將 API 填入 `config.ini` 中的 `API_KEY` 欄位
## 使用方式
1. 啟動伺服器
```bash
python app.py
```
2. 開啟瀏覽器並前往 http://127.0.0.1:5000
3. 上傳照片、輸入活動內容 &rarr; 點選「產生學習歷程」
4. 自動下載生成的 Word 報告
## 作者（依姓氏筆劃排序）
- 宋宣錕
- 張睿玹
- 陳欣妤
- 蔡淳宇
## 法律聲明
- 本專案使用之 **Google Gemini API** 需依照 Google 官方服務條款使用，請自行確認金鑰申請與使用規範
- 產生的內容僅供參考，作者對其正確性與完整性不負任何保證
- 使用本專案所造成的任何法律責任或爭議，皆由使用者自行承擔
- 作者保留隨時修改、移除或中止本專案的權利