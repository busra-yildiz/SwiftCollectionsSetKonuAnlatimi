# SwiftCollectionsSetKonuAnlatimi
Set, benzersiz öğelerin koleksiyonunu tutan bir veri yapısıdır. Bu öğeler, sırasızdır ve her bir öğe yalnızca bir kez bulunabilir. Set'ler, özellikle 
veri tekrarı olmadan benzersiz öğeleri saklamak için kullanışlıdır. İşte Swift dilinde Set kullanımına dair temel bilgiler:

Set Oluşturma:
Swift'te bir Set oluşturmak için çeşitli yollar vardır. İşte birkaç örnek:
// Boş bir Set oluşturma
var emptySet = Set<String>()

// Literallerle Set oluşturma
var fruits: Set<String> = ["Elma", "Muz", "Üzüm"]

// Tür belirtmeden Set oluşturma (Tür çıkarımı kullanarak)
var colors = Set(["Kırmızı", "Yeşil", "Mavi"])

Set Öğelerine Erişim:
Bir Set içindeki öğelere erişmek için for döngüsü veya contains yöntemini kullanabilirsiniz. Örnekler:

// Set içinde dolaşma
for fruit in fruits {
    print(fruit)
}

// Belirli bir öğenin Set içinde olup olmadığını kontrol etme
if colors.contains("Kırmızı") {
    print("Kırmızı renk bulundu.")
}

Set İşlemleri:
Set'lerde temel işlemler şunlarla sınırlıdır: ekleme, çıkarma ve güncelleme.
Öğe Ekleme:

fruits.insert("Çilek")

Öğe Çıkarma: 
colors.remove("Yeşil")

Set İşlemleri:
Set'ler arasında birleşim, fark ve kesişim gibi işlemler yapabilirsiniz. İşte örnekler:
Birleşim:
let set1: Set<Int> = [1, 2, 3]
let set2: Set<Int> = [3, 4, 5]
let unionSet = set1.union(set2) // [1, 2, 3, 4, 5]
Fark:
let differenceSet = set1.subtracting(set2) // [1, 2]
Kesişim:
let intersectionSet = set1.intersection(set2) // [3]

Bu temel Set işlemleri, Swift programlama dilinde Set kullanımına ilişkin önemli bir başlangıç ​​noktasıdır. Set'ler, özellikle benzersiz öğeleri 
takip etmeniz gereken durumlarda kullanışlıdır ve diğer koleksiyon türleri gibi birçok farklı işlemi destekler.
