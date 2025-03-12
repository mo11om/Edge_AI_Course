**第十四講的主題是實作案例 ─ 異常偵測 (Implementation Case - Anomaly Detection)**.


*   **課程大綱**:
    *   14.1. 異常偵測技術簡介
    *   14.2. 異常偵測開源資源
    *   14.3. 常見MCU AI視覺模組
    *   14.4. 異常影像偵測案例

*   **何謂異常偵測（離群偵測）**：
    *   異常偵測的目標是找出與大多數資料不同的離群點。

*   **常見異常偵測作法**:
    *   **一元異常偵測 (One-class Anomaly Detection)**：例如基於支持向量機式的方法，像是 **支持向量數據描述 (Support Vector Data Description, SVDD)**，它透過找出一個超球體來包圍所有已知的正常數據，任何在此球體外的數據則被視為異常.
    *   **時序異常偵測 (Time-series Anomaly Detection)**：當感測器資料（如溫度、濕度、馬達震動等）在時間序列上出現與正常模式顯著不同的行為時，則判定為異常.
    *   **影像異常偵測（瑕疵檢測） (Image Anomaly Detection / Defect Detection)**：在影像中檢測不正常的區域或物件，例如工業產品的瑕疵. 這可以進一步分為分類、物件偵測和分割等方法.

*   **異常偵測的挑戰**:
    *   在工業界等應用中，**好的或正常的樣本通常容易收集，但壞的或異常的樣本往往很難收集到足夠的數量**，這使得傳統需要正負樣本的監督式學習方法面臨挑戰.

*   **常見MCU AI視覺模組 (2024)**:
    *   課程提到了常見的微控制器 (MCU) AI視覺模組，並列舉了一些型號，例如 NXP i.MX RT1062、Seeed Xiao ESP32 Sense、STM32N6、Renesas EK-RA8D1.
    *   特別提到了 **Seeed Vision AI Module V2**，它使用了 **Himax（奇景） WiseEye2** 晶片，該晶片具有雙核心 Arm Cortex-M55 和一個 Micro NPU Ethos-U55.

*   **異常影像偵測案例**:
    *   **Edge Impulse FOMO-AD**：這是一種基於 **FOMO (Faster Objects, More Objects)** 和 **GMM (Gaussian Mixture Model)** 的視覺異常偵測方法.
        *   FOMO-AD 的流程包括資料採集 (區分 "no anomaly" 和 "anomaly" 影像)、Impulse 設計、模型訓練和即時測試.
        *   Edge Impulse 提供了相關的學習模組、說明文章和公開範例. 您可以將公開範例複製到個人帳號中執行.
    *   **水五金異常偵測案例**：這是一個使用 Seeed Vision AI Module V2 和 Seeed SenseCraft 應用程式的案例.
    *   **Seeed SenseCraft AI**：這是一個平台，可以選擇裝置和模型，並進行模型部署、連接、上傳和測試.

*   **開源資源**:
    *   課程提到了異常偵測的開源資源，並在案例部分重點介紹了 Edge Impulse 的 FOMO-AD.

*   **延伸閱讀**:
    *   講師 許哲豪 (Jack Hsu) 在其 AI HUB 專欄中撰寫了多篇關於導入 AI 異常偵測技術於智慧製造的文章，涵蓋時序型資料、表面瑕疵、生成對抗網路 (GANs)、深度學習裂縫檢測以及深度度量學習等主題.

總之，第十四講聚焦於**異常偵測**這個在邊緣 AI 和 TinyML 領域非常重要的應用。課程介紹了異常偵測的基本概念、常見方法（特別是一元異常偵測）、可用的開源資源以及基於 MCU 的視覺異常偵測案例，例如使用 Edge Impulse FOMO-AD 和 Seeed Vision AI Module V2 進行實作. 講師也強調了異常樣本收集的挑戰以及學習正常樣本特徵以進行異常判斷的思路.