**第十一講的主題是實作案例 ─ 姿態估測 (Pose Estimation)**。

在這一講中，講師 Jack 主要介紹了**姿態估測的相關技術與應用**，並著重於在邊緣 AI 上的應用。以下是根據逐字稿整理的重點：

*   **姿態估測的概念**：課程提到了模仿 **COCO (Common Objects in Context) 資料集**的做法來進行姿態估測，並區分了 **二維和三維的表示方法**。二維表示僅包含 X、Y 座標，而三維表示則多了可見性 (visible) 的資訊。V8 模型與 COCO 的關鍵點 (key point) 基本相同。

*   **Intel OpenVINO 與姿態估測**：課程簡略提到了 Intel OpenVINO 在姿態估測上的應用，並指出 OpenVINO 常用的模型來自 OPP 或其他框架。

*   **MediaPipe 的介紹**：課程重點介紹了 **Google 的 MediaPipe** 作為一個更方便且輕量級的解決方案，**特別適合在邊緣設備上使用**。
    *   **輕量化特性**：MediaPipe 非常輕量，可以在 CPU 上運行，因此適用於樹莓派 (Raspberry Pi) 或手機等 CPU 效能相對較弱的設備。若設備有 GPU，效能會更好。
    *   **多平台支援**：MediaPipe 支援多種平台，包括 Android、iOS、Python 和 Web 等。
    *   **豐富的功能**：MediaPipe 提供了非常多且完整的功能，涵蓋視覺、文字和聲音等多個方面。在視覺方面，包括了**影像分類**、**物件偵測**、**人臉辨識**、**影像分割**，甚至還包括了交互式分割 (Interactive Segmentation，類似之前課程提到的 SAM) 和人像美化等。最近還新增了生成式模型 (Generative Models) 的部分，但目前只有少數幾項。
    *   **低程式碼與無程式碼 (LOC & No-Code)**：MediaPipe 的一個主要特色是可以用很少的程式碼 (LOC) 就能實現所需功能，甚至可以完全使用其介面進行操作 (No-Code)，方便使用者練習和測試。
    *   **廣泛的應用案例**：MediaPipe 提供了許多相關的案例，例如手部特徵點偵測 (hand keypoint detection)。
 