# IELTS Speaking Mobile AI Web

這是一個手機可用的 IELTS Speaking 題庫＋AI 自由問答網站。

## 功能
- 手機 / 平板 / 電腦 responsive
- Part 1 / Part 2 / Part 3 題庫
- 搜尋、展開、隨機抽題
- 自由輸入中文或英文 IELTS Speaking 題目
- 可輸入自己的個人例子
- AI 依照「簡單英文 + Band 9 thinking + 繁中翻譯」回答

## 重要
不要把 OpenAI API Key 寫在 public/index.html。
API Key 必須放在 Vercel Environment Variables。

## 部署到 Vercel

1. 建立 GitHub repository，把這個專案全部上傳。
2. 登入 Vercel，選 Add New -> Project。
3. Import 你的 GitHub repository。
4. 在 Project Settings -> Environment Variables 新增：
   OPENAI_API_KEY = 你的 API Key
5. 可選：
   OPENAI_MODEL = gpt-5
6. Deploy。
7. Vercel 會給你一個 https://xxxx.vercel.app 網址。
8. 用 iPhone / Android 打開這個網址即可使用。

## 本機測試
安裝 Node.js 與 Vercel CLI 後：

npm install
npm install -g vercel
vercel dev

然後開瀏覽器：
http://localhost:3000

## iPhone
Safari 開啟部署後網址 -> 分享 -> 加入主畫面。

## Android
Chrome 開啟部署後網址 -> 選單 -> 加到主畫面 / Install app（依瀏覽器顯示）。

## API 費用
ChatGPT 訂閱與 OpenAI API 是分開計費的。需要另外在 OpenAI API Platform 設定 API billing。
