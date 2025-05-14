# 🕶️ VAE Glasses Removal – VAE-GAN Hybrid
Variational Autoencoder (VAE) with a Generative Adversarial Network (GAN) to produce more realistic, glasses-free facial images.

> 📚 系列作品｜Project Series:
> - [Part 1: Basic VAE](https://github.com/VanessaTsai0828/vae-remove-glasses)
> - [Part 2: Grayscale VAE](https://github.com/VanessaTsai0828/vae-remove-glasses-gray)
> - [Part 3: VAE with VGG loss](https://github.com/VanessaTsai0828/vae-remove-glasses-vgg)
> - [Part 4: VAE-GAN](https://github.com/VanessaTsai0828/vae-remove-glasses-gan)

---

## 🧠 專案內容 | What’s Inside
- 使用 VAE 做為生成器（Generator），GAN 加入判別器（Discriminator）
- 損失包含：重建誤差 + KL 散度 + 對抗損失（Adversarial Loss）
- 模型訓練極度不穩定，但具有挑戰性與實驗價值
- 輸出圖像有時會偏移、變形，但也有去除眼鏡的潛力
- Uses a VAE as the generator, with a discriminator added from GAN
- Loss includes: reconstruction error + KL divergence + adversarial loss
- Training is highly unstable, but provides experimental and technical value
- Output images may be distorted or shifted, but still show potential for glasses removal

---

## 📸 範例結果 | Sample Result
![image](https://github.com/user-attachments/assets/01907e0d-d933-41d6-b6cf-9f0c0e69ee0e)



---

## 📌 備註 | Notes
- 此版本訓練不穩，臉型變形是正常現象 🙃
- 判別器和 VAE 同時訓練需要非常謹慎的平衡
- 可作為了解 adversarial training 陷阱與挑戰的實驗素材
- This version is unstable; distorted facial shapes are expected 🙃
- Simultaneously training the discriminator and VAE requires delicate balance
- Useful for exploring the challenges and pitfalls of adversarial training


### 😅 開發者內心話｜Self-Roast Corner
- 我只是想讓臉更真實一點...但模型選擇了自由發揮。  如果你知道怎麼讓這包不崩壞，請告訴我～拜託了 🙏
- I just wanted to make the face look more realistic... but the model decided to express itself freely.
  If you know how to make this version less broken, please tell me. Thank you. 🙏
