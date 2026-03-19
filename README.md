# MuratKUS
# Larenks 3B Modelleme - 3D Larynx Modeling

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-1.9+-red.svg)](https://pytorch.org/)

Bu depo, **"Açık Kaynaklı Yapay Zekâ Tabanlı 3B Larenks Modellemesi"** başlıklı akademik çalışmaya ait kaynak kodlarını içermektedir. Çalışma, tıbbi görüntüleme verilerinden (BT/MR) yapay zekâ kullanarak larenksin üç boyutlu modellerini otomatik olarak oluşturan açık kaynaklı bir sistem sunmaktadır.

---

## 📋 İçindekiler
- [Özellikler](#-özellikler)
- [Kullanılan Teknolojiler](#-kullanılan-teknolojiler)
- [Kurulum](#-kurulum)
- [Kullanım](#-kullanım)
- [Veri Seti](#-veri-seti)
- [Sonuçlar](#-sonuçlar)
- [Dosya Yapısı](#-dosya-yapısı)
- [Lisans](#-lisans)
- [Atıf](#-atıf)
- [İletişim](#-iletişim)

---

## ✨ Özellikler

- ✅ **Otomatik Segmentasyon**: 3B U-Net derin öğrenme modeli ile larenks anatomisinin otomatik olarak ayrıştırılması
- ✅ **Çoklu Yapı Desteği**: Vokal kıvrımlar, tiroid kıkırdak, krikoid kıkırdak, aritenoid kıkırdaklar ve epiglot segmentasyonu
- ✅ **Yüzey Çıkarımı**: Marching Cubes algoritması ile hacimsel verilerden 3B yüzey ağları oluşturma
- ✅ **Mesh Optimizasyonu**: Laplacian/Taubin yumuşatma ve çokgen sadeleştirme ile hafif ve kullanılabilir modeller
- ✅ **Açık Kaynak**: Tüm kodlar MIT lisansı ile ücretsiz olarak sunulmaktadır
- ✅ **Modüler Yapı**: Kolayca genişletilebilir ve farklı anatomik bölgelere uyarlanabilir

---

## 🛠 Kullanılan Teknolojiler

| Teknoloji | Amaç |
|:---|:---|
| **Python 3.8+** | Ana programlama dili |
| **PyTorch** | Derin öğrenme modeli eğitimi |
| **3B U-Net** | Segmentasyon mimarisi |
| **ITK/SimpleITK** | Tıbbi görüntü işleme |
| **VTK** | 3B görselleştirme ve yüzey çıkarımı |
| **Marching Cubes** | Yüzey çıkarım algoritması |
| **Blender** | Mesh optimizasyonu ve görselleştirme |

---

## 🚀 Kurulum

### Gereksinimler
- Python 3.8 veya üzeri
- CUDA destekli GPU (opsiyonel, hız için)

### Adımlar

1. **Depoyu klonlayın**
```bash
git clone https://github.com/murathan0201-tech/MuratKUS.git
cd MuratKUS
