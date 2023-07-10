# Machine-learning-knn-ile-hesaplama
Bu kod örneği, K-En Yakın Komşu (KNN) algoritmasını kullanarak bir veri setinde sınıflandırma yapmayı göstermektedir. İşleyişi şu şekildedir:

    İlk olarak, math ve collections kütüphaneleri import edilir ve pandas kütüphanesi pd takma adıyla import edilir.
    ---------------------------------
    Excel'den veri seti yüklenir. data_file değişkeni, veri setinin dosya yolunu içermelidir. pd.read_excel() fonksiyonu kullanılarak veri seti bir DataFrame olarak df değişkenine yüklenir.
      ---------------------------------
    Giriş özellikleri (X) belirlenir. Burada, df DataFrame'indeki ilgili sütunlar seçilerek bir numpy dizisine dönüştürülür.
      ---------------------------------
    Öklidyen mesafesini hesaplamak için euclidean_distance() fonksiyonu tanımlanır. Bu fonksiyon, iki vektör arasındaki öklidyen mesafesini hesaplar.
      ---------------------------------
    KNN algoritmasını uygulamak için knn_predict() fonksiyonu tanımlanır. Bu fonksiyon, bir test verisi için en yakın komşuları bulur, komşuların sınıflarını sayar ve en yaygın sınıfı tahmin olarak döndürür.
      ---------------------------------
    Kullanıcıdan test veri seti girişleri alınır. for döngüsü ile her bir özellik için kullanıcıdan değerler alınır ve test_data listesine eklenir.
  ---------------------------------
    K değeri belirlenir. k değişkeni, KNN algoritmasında kaç komşunun kullanılacağını belirlemek için kullanılır.
  ---------------------------------
    Tahmin yapmak için knn_predict() fonksiyonu çağrılır ve sonuç tahminini prediction değişkenine atar.
  ---------------------------------
    K değeri içeren öklidyen mesafeleri ve komşuları yazdırır.
  ---------------------------------
    Tahmini ekrana yazdırır.

Bu kod örneği, KNN algoritmasını anlamak ve uygulamak için bir temel sağlar. Veri setinizi ve ilgili sütunları uygun şekilde güncelleyerek kendi verileriniz üzerinde KNN algoritmasını çalıştırabilirsiniz.
