# Sudoku Quest｜數獨闖關

一款純前端、可部署到 GitHub Pages 的經典數獨遊戲。無需安裝套件或後端服務。

## 功能
- 9×9 經典數獨棋盤，3×3 宮格分隔線與選取高亮
- 動態生成數獨題目，生成後會檢查唯一解
- 提示：將選取空格填入正確答案
- 橡皮擦：清除玩家輸入，不會修改題目固定數字
- 筆記模式：每格可標記 1–9 候選數字
- 錯誤與重複數字提醒、棋盤檢查
- 計時、撤銷、重新開始、新遊戲
- Easy、Medium、Hard、Expert 四級闖關與最佳時間
- 使用 localStorage 自動保存本機遊戲進度
- 響應式版面，支援手機與桌面瀏覽器

## 本機遊玩
直接用瀏覽器開啟 `index.html` 即可。若瀏覽器限制本機儲存，可使用 VS Code Live Server 等靜態伺服器。

## 部署到 GitHub Pages
1. 在 GitHub 建立新的 repository，例如 `sudoku-quest`。
2. 上傳 `index.html` 與 `README.md` 至 repository 根目錄。
3. 打開 repository 的 **Settings → Pages**。
4. 在 **Build and deployment** 中選擇 **Deploy from a branch**。
5. Branch 選 `main`，資料夾選 `/(root)`，按 Save。
6. 等待部署完成，GitHub Pages 會顯示網站網址，通常形式為 `https://你的帳號.github.io/sudoku-quest/`。

## 操作
- 點選空格，再點右側數字或使用鍵盤 `1`–`9`。
- `Backspace` / `Delete` 清除選取格。
- `N` 切換筆記模式。
- 方向鍵移動選取格。
- 提示會填入正確數字並扣除一次提示額度。

## 備註
- 遊戲紀錄存在目前瀏覽器的 `localStorage`，不會自動跨裝置同步。
- 每局題目以隨機完整解盤為基礎移除數字，並以解數計數器確保唯一解。
- 難度以題目線索數作初步區分；不同題目的實際推理難度仍可能略有差異。
