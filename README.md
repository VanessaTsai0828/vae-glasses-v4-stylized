# 🕶️ VAE Glasses Removal – GAN Version  
Integrated GAN discriminator into the VAE architecture for enhanced realism.  
Includes KL warm-up, KL loss clipping, and increased GAN loss weight for training stability.


> 📚 系列作品｜Project Series:
> - [Part 1: Baseline VAE](https://github.com/VanessaTsai0828/vae-glasses-v1-baseline)
> - [Part 2: Grayscale VAE](https://github.com/VanessaTsai0828/vae-glasses-v2-grayinput)
> - [Part 3: VAE with VGG Loss](https://github.com/VanessaTsai0828/vae-glasses-v3-vggloss)
> - [Part 4: VAE with GAN](https://github.com/VanessaTsai0828/vae-glasses-v4-gan)

---

## 🧠 專案內容 | What’s Inside
- 使用 VAE 做為生成器（Generator），加入 GAN 判別器（Discriminator）
- 損失函數包含：重建誤差 + KL 散度（warm-up）+ 對抗損失（GAN Loss）
- 為避免不穩定訓練，加入 KL warm-up 與 clip 限制 KL 最大值
- 調整 GAN loss 權重為 5.0，使對抗訓練穩定收斂
- Uses a VAE as the generator, with an adversarial discriminator from GAN
- Loss = Reconstruction + KL divergence (with warm-up) + GAN loss
- KL warm-up and clipping stabilize the training and prevent KL explosion
- Increased GAN loss weight (5.0) helps improve adversarial convergence

---

## 📸 範例結果 | Sample Result
![image](https://github.com/user-attachments/assets/16ae2129-a75c-4f71-92d1-4958f79e33fc)
![image](https://github.com/user-attachments/assets/106bf876-02ab-4524-8c26-c7d615b1b4aa)


---

## 📌 備註 | Notes
- 本版本為最終穩定版本，可實際用於 glasses removal 實驗或展示
- 若需產出圖片，建議在訓練結束後執行 decoder(z) 並可視化
- 為節省資源，本專案預設不在訓練中進行圖像輸出
- This version is stable and suitable for experiments or demonstrations
- Images can be generated from decoder(z) after training
- To save resources, image output is disabled during training by design
