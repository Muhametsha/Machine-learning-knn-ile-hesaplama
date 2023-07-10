import math
from collections import Counter
import pandas as pd

# Veri setini Excel'den yükleme
data_file = '/content/ornek(3)(1)(2).xlsx'
df = pd.read_excel(data_file)

print(df)


# Giriş özelliklerini  belirleme
X = df[['egg', 'milk', 'fish', 'wheat', 'sellfish', 'Peanuts','hasta']].values


# Öklidyen mesafesini hesaplamak için formul
def euclidean_distance(vector1, vector2):
    squared_diff = [(v1 - v2) ** 2 for v1, v2 in zip(vector1, vector2)]
    distance = math.sqrt(sum(squared_diff))
    return distance

# KNN algoritmasını uygula
def knn_predict(test_data, training_data, k):
    neighbors = []

    for instance in training_data:
        distance = euclidean_distance(test_data, instance[:-1])
        label = instance[-1]
        neighbors.append((distance, label))
       
    neighbors.sort(key=lambda x: x[0])  # Uzaklığa göre sırala kucukten buyuge

    k_nearest_neighbors = neighbors[:k]  # En yakın K komşuyu seç

    # Komşuların sınıflarını say
    class_count = Counter(neighbor[1] for neighbor in k_nearest_neighbors)

    # Sınıf sayılarına göre tahmini yap
    prediction = class_count.most_common(1)[0][0]
    
    # K değerini içeren öklidyen mesafelerini ve komşuları yazdır
    print(f"K={k} için Öklidyen Mesafeleri ve etiket:")
    for neighbor in k_nearest_neighbors:
        print("Öklidyen Mesafe:", neighbor[0], "etiket:", neighbor[1])

    
    return prediction

# Test veri setini oluşturma giriş
test_data = []
for feature in ['egg', 'milk', 'fish', 'wheat', 'sellfish', 'Peanuts']:
    value = float(input(f"{feature} değerini girin: "))
    test_data.append(value)
# KNN algoritması için K değeri
k = 3


# Tahmin yapmak için
prediction = knn_predict(test_data, X, k)

print("Tahmin:", prediction)
