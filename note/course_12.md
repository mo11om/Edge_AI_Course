**第十二講的主題是實作案例 ─ 語音辨識**。

在這一講中，講師 Jack 從歐尼克斯實境互動工作室的角度，介紹了**如何利用 TinyML 進行語音辨識的實作**。以下是根據講義和逐字稿整理的重點：

*   **TinyML 回顧**：課程開始時會簡要回顧 TinyML 的概念。相關的課程簡報連結也提供在講義中。

*   **簡報大綱**：第十二講的簡報大綱涵蓋了以下幾個部分：
    *   **智慧物聯網與感測技術 (Smart IoT and Sensing Technology)**
    *   **喚醒詞技術簡介 (Keyword Spotting/Wake Word Technology Introduction)**
    *   **TinyML 開發流程與環境 (TinyML Development Flow and Environment)**
    *   **Edge Impulse 喚醒詞案例 (Edge Impulse Keyword Spotting Case Study)**

*   **實作案例 ─ 語音辨識**：課程的核心是透過實作案例來演示語音辨識的應用，特別是**喚醒詞技術**。講師介紹了如何使用 **Edge Impulse** 這個平台來建立和部署 TinyML 語音辨識模型.

*   **Edge Impulse 平台介紹與應用**:
    *   **方便性**：講師強調 Edge Impulse 提供了一個非常方便的平台，可以從資料收集、模型訓練到部署一站式完成語音辨識的專案。
    *   **豐富的範例**：Edge Impulse 提供了各式各樣的語音辨識範例，從簡單的喚醒詞辨識到更複雜的語音指令辨識都有。講師建議使用者可以直接參考這些範例進行學習。
    *   **免費方案限制**：講師也提到了 Edge Impulse 免費方案的一些限制，例如專案數量、資料集大小和模型訓練時間等。他建議初學者可以先利用免費方案練習，如果專案需求較大再考慮付費方案或移回本地端開發。
    *   **資料收集**：課程介紹了如何在 Edge Impulse 上收集語音資料，可以直接上傳預先準備好的 WAV 檔案（非壓縮格式），或者使用 Edge Impulse 提供的工具進行錄音。講師也分享了 Google Speech Commands 資料集的一個迷你版本供練習使用。
    *   **模型訓練與部署**：課程講解了在 Edge Impulse 上進行資料標註、模型設計、訓練和驗證的步驟。針對部署部分，講師示範了如何將訓練好的模型部署到微控制器 (MCU) 上，例如 XIAO nRF52840 (Sense) 開發板。Edge Impulse 會將模型打包成一個函式庫 (Library)，方便在 MCU 上使用。講師也提到部署時可以選擇將浮點數模型量化為整數模型 (例如 INT8) 以減小模型大小和加速推論。
    *   **支援的硬體**：Edge Impulse 支援多種微控制器開發板，使用者可以在平台上選擇適合自己的硬體。

*   **本地開發環境**：講師也簡要提到了本地開發環境的準備，例如 Python 版本和 Node.js 版本的要求，以及如何使用 Edge Impulse 的 CLI (Command Line Interface) 工具將本地資料同步到雲端平台.

