#Machine-learning-knn-ile-hesaplama (Calculation with KNN using machine learning)

This code example demonstrates how to perform classification using the K-Nearest Neighbors (KNN) algorithm on a dataset. Here is how it works:

    First, the math and collections libraries are imported, and the pandas library is imported as pd.

    The dataset is loaded from Excel. The data_file variable should contain the file path of the dataset. The pd.read_excel() function is used to load the dataset into a DataFrame named df.

    The input features (X) are determined. Here, relevant columns in the df DataFrame are selected and converted into a numpy array.

    The euclidean_distance() function is defined to compute the Euclidean distance between two vectors. This function calculates the Euclidean distance.

    The knn_predict() function is defined to implement the KNN algorithm. This function finds the nearest neighbors for a test data point, counts the classes of the neighbors, and returns the most common class as the prediction.

    Test data inputs are taken from the user. For each feature, values are taken from the user using a for loop and added to the test_data list.

    The value of K is determined. The k variable is used to specify the number of neighbors to be used in the KNN algorithm.

    The knn_predict() function is called to make predictions, and the result is assigned to the prediction variable.

    It prints the Euclidean distances and neighbors with the K value.

    It prints the prediction to the screen.

This code example provides a basic understanding and implementation of the KNN algorithm. By updating your dataset and relevant columns accordingly, you can run the KNN algorithm on your own data.


-----------------------------------------------------------------------------------------------------------------------------


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
