# Deep Learning Project

## 🎯 Projenin Amacı
Bu proje, Intel Image Classification veri seti kullanılarak farklı doğal ve yapay ortamları (Buildings, Forest, Glacier, Mountain, Sea, Street) CNN tabanlı modeller ile sınıflandırmayı amaçlamaktadır. 

## 📊 Veri Seti
- Kaynak: [Intel Image Classification Dataset](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)  
- Eğitim: ~25.000 görüntü  
- Test: ~14.000 görüntü  
- Sınıflar: Buildings, Forest, Glacier, Mountain, Sea, Street  

## 🧠 Kullanılan Yöntemler
- CNN tabanlı model (Conv2D, Pooling, Dense, Dropout, Softmax)  
- Data Augmentation (rotation, zoom, flip, shift)  
- Callbacks: ModelCheckpoint, EarlyStopping, ReduceLROnPlateau, TensorBoard  
- Hiperparametre optimizasyonu: farklı filtre sayıları & learning rate denemeleri  
- Değerlendirme: Accuracy & Loss grafikleri, Confusion Matrix, Classification Report  

## ✅ Sonuçlar
- **En iyi doğruluk:** ~81.28% (validation accuracy)  
- **En başarılı yapı:** `filters=64, learning_rate=5e-4`  

### Test Sonuçları
- Genel doğruluk: **85%** (3000 örnek)

| Sınıf      | Precision | Recall | F1-Score | Support |
|------------|-----------|--------|----------|---------|
| Buildings  | 0.83      | 0.84   | 0.83     | 437     |
| Forest     | 0.94      | 0.97   | 0.96     | 474     |
| Glacier    | 0.87      | 0.75   | 0.80     | 553     |
| Mountain   | 0.81      | 0.78   | 0.79     | 525     |
| Sea        | 0.81      | 0.92   | 0.86     | 510     |
| Street     | 0.86      | 0.87   | 0.87     | 501     |

**Macro Avg:** Precision=0.85, Recall=0.85, F1=0.85  
**Weighted Avg:** Precision=0.85, Recall=0.85, F1=0.85  


## 🔗 Notebook
[Kaggle Notebook Linki](https://www.kaggle.com/code/hseyinyilmaz/akbank-derin-ogrenme)
