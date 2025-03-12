**course2**的主題是**邊緣運算硬體**。 

*   **邊緣運算硬體的分類**：邊緣運算硬體可以根據其運算能力和功耗等特性進行分類。在第二講中，MCU（微控制器單元）被歸類為 Tiny 級別。這個領域每年都有競賽，鼓勵開發者提交創新的演算法.
*   **開發語言的考量**：在 MCU 等級的開發中，C 語言由於其效率通常是必要的，尤其是在沒有作業系統的環境下。相較之下，在手機或 AI 晶片上可能運行 Linux 等作業系統。雖然許多開發者習慣使用 Python，但在 MCU 領域可能更具挑戰性.
*   **加速處理單元 (Accelerated Processing Units)**：除了 CPU，邊緣運算硬體可能會包含加速處理單元以提升運算效能，例如 NVIDIA 的 CUDA 或其他類似技術。
*   **開源框架的演變**：講者提到了一些開源深度學習框架，例如 TensorFlow 和 PyTorch。他指出，在邊緣運算領域，TensorFlow Lite 和 ONNX (Open Neural Network Exchange) 是比較常見的選擇。OpenVINO 也被提及，它負責將不同框架開發的模型轉換並部署到特定的硬體上. 然而，一些早期的框架如 Caffe 和 Torch 已經整合到 TensorFlow 和 PyTorch 中，而其他一些則不再活躍或有新的發展.
*   **硬體選用的比喻**：講者用交通工具來比喻不同硬體的適用場景。例如，用腳踏車來執行汽車等級的任務會很困難，但如果對腳踏車進行適當的優化（如同軟體優化），則有可能達到更好的效能.
*   **OpenVINO 的支援**：針對聽眾提問 OpenVINO 是否支援多種模型格式，講者說明 OpenVINO 本身並非直接支援多種模型，而是透過轉換工具將不同框架（如 TensorFlow、PyTorch、ONNX）訓練出的模型轉換為其的 IR (Intermediate Representation) 格式，然後再部署到不同的硬體上. 他也提到 TensorFlow Lite 和 NVIDIA TensorRT 等也具備模型轉換和壓縮的功能.
*   **NPU 的支援**：講者也提到一些針對特定硬體的優化和支援，例如針對聯發科 (MediaTek) NPU 的支援可能需要使用特定的安裝方式. 未來，OpenCV 有可能直接呼叫 NPU 進行加速.

 