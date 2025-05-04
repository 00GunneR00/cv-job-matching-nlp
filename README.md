🧠 CV - İş İlanı Eşleşmesi (Doğal Dil İşleme Projesi)

Bu proje, doğal dil işleme teknikleri kullanılarak aday CV'leri ile iş ilanları arasındaki metinsel uyumu ölçmeyi amaçlamaktadır. Her ilan için en uygun 5 CV önerisi sunulmaktadır.

📁 Proje Yapısı

📂 data/
    ├── cv_dataset.csv
    ├── job_postings.csv
    ├── cv_stemmed.csv
    ├── job_stemmed.csv
    ├── cv_lemmatized.csv
    └── job_lemmatized.csv

📂 models/
    └── cv_stemmed_model_cbow_window2_dim100.model

📂 outputs/
    ├── tfidf_stemmed_cv.csv
    ├── tfidf_stemmed_job.csv

📄 notebook.ipynb
📄 README.md



🧪 Kullanılan Yöntemler

✅ 1. Veri Ön İşleme

Küçük harfe dönüştürme

Noktalama kaldırma

Stopword temizleme (Türkçe)

Tokenizasyon

Lemmatization & Stemming

✅ 2. Zipf Yasası Analizi

Hem ham hem temizlenmiş veri için Zipf dağılımı grafikleri

✅ 3. Vektörleştirme

TF-IDF ile belge-temsil matrisleri

Word2Vec ile kelime gömme (embedding) modeli

✅ 4. Eşleşme Analizi

Word2Vec vektörlerine ortalama alınarak cümle vektörü oluşturuldu

cosine similarity kullanılarak her iş ilanı için en uygun 5 CV belirlendi

🔍 Kullanılan Kütüphaneler

pandas, numpy, matplotlib

nltk, gensim, scikit-learn

spacy (ön model denemeleri)

SnowballStemmer (Türkçe için)

🚀 Nasıl Çalıştırılır?

Gerekli kütüphaneleri yükleyin:

pip install pandas nltk gensim scikit-learn matplotlib

Veri dosyaları data/ klasörüne yerleştirin.

Jupyter Notebook’u çalıştırın:

jupyter notebook

notebook.ipynb dosyasını açarak adım adım çalıştırabilirsiniz.

🎯 Proje Amacı

Bu proje, İnsan Kaynakları süreçlerinde metin tabanlı eşleşme sistemlerinin nasıl geliştirilebileceğini göstermek amacıyla hazırlanmıştır. Doğal dil işleme yöntemlerinin gerçek bir senaryoda uygulanması hedeflenmiştir.

📌 Notlar

Veriler yapay olarak oluşturulmuş ya da düzenlenmiştir.

Geliştirme ve test için uygun hale getirilmiş Türkçe metinler içerir.

Daha iyi lemmatization için Zemberek veya Stanza gibi Türkçe araçlar entegre edilebilir.



Güner Bektaş
