---
tags: Stable Diffusion
description: Stable Diffusion 相關資源
---

# Stable Diffusion 相關資源
## Stable Diffusion Web UI
* [GitHub](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
* LICENSE [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.en.html)

## 反向提詞 
#### 模組
* [EasyNegative](https://civitai.com/models/7808)  
反提詞：`easynegative,`
* [Deep Negative V1.x](https://civitai.com/models/4629)  
反提詞：`ng_deepnegative_v1_75t,`
* [Bad artist Negative embedding](https://civitai.com/models/5224)  
反提詞：sketch by bad-artist,painting by bad-artist,photograph by bad-artist,  
反提詞：sketch by bad-artist-anime,painting by bad-artist-anime,photograph by bad-artist-anime,  

#### 咒語
**halftone**  
反提詞：`(halftone:2),`  
作用於：半色調修正  

**pixels**  
反提詞：`(pixels:2),`  
作用於：減少嘈雜的像素點（減少雜訊）  

**asymmetric**  
反提詞：`(asymmetric:1.5),`  
作用於：減少不對稱問題  

###### 標準版（二次元特化）
```
ng_deepnegative_v1_75t,easynegative,sketch by bad-artist-anime,painting by bad-artist-anime,photograph by bad-artist-anime,
(halftone:2),(pixels:2),(asymmetric:1.5),nsfw,
```

###### 加強版（二次元特化）
```
ng_deepnegative_v1_75t,easynegative,sketch by bad-artist-anime,painting by bad-artist-anime,photograph by bad-artist-anime,
(halftone:2),(pixels:2),extra hands,missing fingers,broken hand,more than two hands,well proportioned hands,more than two legs,unclear eyes,missing arms,mutilated,extra limbs,extra legs,cloned face,fused fingers,extra digit,fewer digits,extra digits,.jpeg,(artifacts:1.5),(signature:1.5),(watermark:1.5),(username:1.5),mirror image,Vague,paintings,sketches,(worst quality:2),(low quality:2),(normal quality:2),lowres,normal quality,((monochrome)),((grayscale)),skin spots,acnes,skin blemishes,age spot,manboobs,backlight,(ugly:1.331),(duplicate:1.331),(morbid:1.21),(mutilated:1.21),(tranny:1.331),mutated hands,(poorly drawn hands:1.331),blurry,(bad anatomy:1.21),(bad proportions:1.331),extra limbs,(disfigured:1.331),(more than 2 nipples:1.331),(missing arms:1.331),(extra legs:1.331),(fused fingers:1.61051),(too many fingers:1.61051),(unclear eyes:1.331),bad hands,missing fingers,extra digit,(futa:1.1),bad body,(asymmetric:1.5),nsfw,
```

## 大模型 CheckPoint 

## 渲染器 VAE 
* [kl-f8-anime2](https://huggingface.co/hakurei/waifu-diffusion-v1-4/blob/main/vae/kl-f8-anime2.ckpt)  
一個很泛用的VAE

## 小模型 Lora 
* [Gacha splash LORA](https://civitai.com/models/13090/gacha-splash-lora)  
![](https://imagecache.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/e1b50fbc-dbea-4376-beae-8d08ed663900/width=320)
* [Standing Full Body with Background Style LoRA](https://civitai.com/models/16997/standing-full-body-with-background-style-lora)  
![](https://imagecache.civitai.com/xG1nkqKTMzGDvpLrqFT7WA/1a728c90-0334-4e86-3c61-c860a4b32800/width=320)

## 擴充元件
> 安裝方式  
> 請到擴充功能（Extensions） > 從網址安裝（Install from URL）  
> 在 擴充功能的 git 倉庫網址（URL for extension's git repository）貼上網址後  
> 按下安裝（Install）等待安裝完成, 並重新載入UI即可  
> （不懂如何重新載入, 可以把小黑窗關掉重開）

#### 性能優化
* [MultiDiffusion](https://multidiffusion.github.io) 算法及 VAE 分塊  
[Tiled Diffusion](https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111.git)

#### 介面（UI）體驗
* 自動提詞補全  
[Tag Autocompletion](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete.git)
* 動態提詞&提詞卡  
[Dynamic Prompts](https://github.com/adieyal/sd-dynamic-prompts.git)
* 雙語系顯示  
[Bilingual Localization](https://github.com/journey-ad/sd-webui-bilingual-localization.git)
* 常用參數記錄  
[Preset Utils](https://github.com/Gerschel/sd_web_ui_preset_utils.git)

#### 色彩修正
* AI色盲處理  
[Cutoff - Cutting Off Prompt Effect](https://github.com/hnmr293/sd-webui-cutoff.git)
#### 套件管理
* Civitai 套件處理  
[Civitai Helper](https://github.com/butaixianran/Stable-Diffusion-Webui-Civitai-Helper.git)

#### 其他
* 美學評分  
[Aesthetic Image Scorer](https://github.com/tsngo/stable-diffusion-webui-aesthetic-image-scorer.git)  
Windows 下需另外安裝相依套件 [FileMeta](https://github.com/Dijji/FileMeta/releases)
