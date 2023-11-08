# Timus-Full-Stack-Bootcamp-Homework-1


## 1. JavaScript nedir ve tarihsel gelişiminden bahsedin
JavaScript, başlangıçta Netscape Communications Corporation tarafından 1995 yılında geliştirilen bir tarayıcı dili olarak ortaya çıktı. Zamanla, web uygulamalarının karmaşıklığı arttıkça, ECMAScript standartları ve AJAX gibi teknolojilerin gelişimiyle JavaScript'in popülaritesi hızla yükseldi. Sonuç olarak, Node.js gibi araçların da ortaya çıkmasıyla JavaScript, sadece tarayıcılar için değil, sunucu taraflı uygulamalar da dahil olmak üzere geniş bir kullanım alanı buldu.

## 2. Java ile javascript arasındaki fark nedir
Java, genellikle büyük ölçekli uygulamalar için kullanılan güçlü bir programlama dilidir. JavaScript ise web tarayıcılarında etkileşimli web sayfaları oluşturmak için kullanılan bir betik dilidir. Java, sunucu taraflı uygulamalardan mobil uygulamalara kadar geniş bir alanda kullanılırken, JavaScript genellikle web geliştirme için kullanılır.

## 3. Javascript teki veri tipleri nelerdir açıklayınız
Veri tipleri iki kategoriye ayrılır:
1.	Primitive (İlkel): Bu kategori, sayılar, metinler, boolean değerler, null ve undefined gibi basit veri türlerini içerir.
2.	Composite (Bileşik): Bu kategori, nesneler, diziler, fonksiyonlar gibi daha karmaşık ve yapılandırılmış veri türlerini içerir. Bu veri türleri, daha karmaşık veri yapıları veya işlevlerin temsil edilmesinde kullanılır.

Temel veri tipleri şunlardır:

1. **Number (Sayı):** Sayısal verileri temsil eder, hem tam sayılar hem de ondalıklı sayılar kullanılabilir. Örneğin: 5, 3.14 gibi.

2. **String (Metin):** Metinsel verileri temsil eder. Tek tırnak (''), çift tırnak ("") veya ters tırnak (`) kullanılarak oluşturulabilir. Örneğin: "Merhaba", 'JavaScript'.

3. **Boolean (Mantıksal):** Sadece iki değer alabilen veri türüdür: true (doğru) veya false (yanlış). Mantıksal durumları temsil etmek için kullanılır.

4. **Null:** Değerin boş veya yok olduğunu belirtir. Bir değişkenin atanmamış veya var olduğu ancak değerinin olmadığı durumlarda null kullanılır.

5. **Undefined:** Değişkenin tanımlanmamış olduğunu belirtir. Bir değişken tanımlanmış ancak değer ataması yapılmamışsa varsayılan olarak undefined değerini alır.

6. **Object (Nesne):** Bu veri türü, karmaşık veri koleksiyonlarını temsil eder. Nesneler, özellik ve değer çiftleri içerebilir. Nesneler, fonksiyonlar, diziler ve daha fazlasını içerebilir.

7. **Array (Dizi):** Verilerin listesini temsil eder. Tek bir değişkende birden çok değer saklamak için kullanılır. Örneğin, [1, 2, 3, 4] gibi.

8. **Function (Fonksiyon):** Bir dizi işlevi gerçekleştiren bir alt programı temsil eder. JavaScript'te fonksiyonlar birinci sınıf nesnelerdir, bu da onları değişkenlere atayabilir, diğer fonksiyonlardan döndürebilir ve argüman olarak iletebilirsiniz.

## 4. null ile undefined arasıdaki fark nedir açıklayınız
JavaScript'te, `null` ve `undefined` farklı anlamlara sahip iki özel değerdir.

1. **null:** Bu değer, bir değişkenin bilerek veya isteyerek boş olduğunu veya bir değer olmadığını belirtmek için kullanılır. Bir değişkenin değerinin var olduğu ancak içeriğinin bilinmediği veya henüz atanmadığı durumlarda `null` değeri atanabilir. Örneğin:

   ```javascript
   let deger = null;
   ```

2. **undefined:** Bu değer, bir değişkenin tanımlanmış olmasına rağmen değerinin atanmamış olduğunu belirtir. Bir değişkenin tanımsız olduğu durumlarda JavaScript, varsayılan olarak `undefined` değerini atar. Örneğin:

   ```javascript
   let isim;
   console.log(isim); // Çıktı: undefined
   ```

Temel farkları şu şekilde özetlenebilir:

- `null`, bilerek boş bir değeri temsil ederken, `undefined` bir değerin atanmamış olmasını temsil eder.
- Bir değişkenin `null` olarak atanmış olması, değerinin bilerek boş olduğu anlamına gelirken, `undefined` olması, değerin atanmamış olduğunu gösterir.
- `null` bir değerdir, ancak `undefined` bir türdür.

## 5. NaN nedir açıklayınız
NaN, "Not-a-Number" kısaltmasıyla bilinen, JavaScript'te bir değerin sayı olmadığını belirtmek için kullanılan bir değerdir. Özellikle matematiksel işlemler sırasında beklenmeyen veya geçersiz bir sonuç elde edildiğinde JavaScript NaN değerini döndürebilir.
Örneğin, bir sayıyı sıfıra bölmeye çalıştığınızda veya sayı olmayan bir ifadeyi sayıya çevirmeye çalıştığınızda (örneğin, bir metin dizesini sayıya dönüştürmeye çalışırken), JavaScript NaN değerini döndürebilir.
javascriptCopy code
let x = 0 / 0; // NaN let y = parseInt("hello", 10); // NaN 
NaN, JavaScript'te bir değerin sayı olmadığını belirtmek için özel bir değerdir. Bu, matematiksel işlemler sırasında hataların veya beklenmeyen sonuçların kontrol edilmesi için kullanışlı bir araçtır. Bu durumlarla karşılaşıldığında, programın düzgün çalışması için uygun hata işleme mekanizmaları kullanılmalıdır.

## 6. Javascript’te yorum satırı eklemenin kaç farklı yolu vardır
JavaScript'te yorum satırları, kodun anlaşılabilirliğini artırmak ve açıklama eklemek için kullanılır. JavaScript'te yorum eklemenin iki farklı yolu vardır:

1. **Tek Satırlı Yorumlar:** Tek satırlı yorumlar, `//` işareti kullanılarak oluşturulur ve bu işaretten sonraki her şey o satırda yorum olarak kabul edilir.

```javascript
// Bu bir tek satırlı yorum örneğidir
let x = 5; // Bu da bir değişken ataması
```

2. **Çok Satırlı Yorumlar:** Çok satırlı yorumlar, `/*` ve `*/` işaretleri arasına alınan her şeyin yorum olarak kabul edilmesini sağlar. Bu şekilde, birden fazla satırda yorum eklemek mümkündür.

```javascript
/*
Bu bir çok satırlı yorum örneğidir.
Birden fazla satırda açıklama yapmak için kullanılabilir.
*/

let y = 10; // Bu da başka bir değişken ataması
```

Bu yorum türleri, kodun ne yaptığını belirtmek, karmaşık veya önemli parçaları açıklamak veya kodun diğer geliştiriciler tarafından daha iyi anlaşılmasını sağlamak için yaygın olarak kullanılır.

## 7. Global değişken ne demektir açıklayınız
Global değişken, bir programın herhangi bir noktasında tanımlanabilen ve bu tanımlandığı andan itibaren herhangi bir fonksiyon veya kapsam tarafından erişilebilen bir değişkendir. JavaScript'te global değişkenler genellikle en dış kapsamda, yani herhangi bir fonksiyon veya blok içinde değil, genel alanda tanımlanır. Bu durumda, değişken tüm kod blokları içinde erişilebilir ve kullanılabilir durumda olur. Ancak, global değişkenlerin fazla kullanımı kod karmaşıklığını artırabilir ve istenmeyen yan etkilere neden olabilir, bu yüzden genellikle sınırlı kullanılmaları tavsiye edilir.

## 8. Javascript’te this anahtar kelimesi nedir açıklayınız
JavaScript'te this anahtar kelimesi, bulunduğu bağlam veya kapsayıcıya bağlı olarak değişen özel bir kelime veya referanstır. this, JavaScript'te kullanıldığında, genellikle şu anda çalışan veya etkileşimde bulunduğunuz nesneyi veya kapsayıcıyı temsil eder. Bu durum, fonksiyonlar, nesneler veya constructor fonksiyonları gibi farklı durumlar için farklı şekillerde davranabilir.
this anahtar kelimesi, bir fonksiyonun içinde kullanıldığında, o anki çalışma bağlamına göre değişebilir. Bu bağlam, fonksiyonun nasıl çağrıldığına bağlıdır. Örneğin, bir fonksiyon bir nesne içinden çağrılıyorsa, this, o nesneyi temsil eder. Ancak aynı fonksiyon bir küresel bağlamda çağrılırsa, this genellikle window nesnesini temsil eder.
Başka bir örnek olarak, constructor fonksiyonlarından oluşturulan nesnelerde this, o an oluşturulan nesneyi temsil eder.

## 9. == ile === farkını örnekler ile açıklayınız
`==` operatörü, JavaScript'te değerlerin eşit olup olmadığını kontrol etmek için kullanılır. Bu operatör, karşılaştırılan değerlerin sadece değerlerini kontrol eder, ancak veri türlerini dikkate almaz. Örneğin:

```javascript
console.log(1 == '1'); // true
console.log(1 == 1); // true
console.log(0 == false); // true
```

`===` operatörü ise hem değerleri hem de veri türlerini kontrol eder. Bu nedenle, `===` operatörü, değerlerin yanı sıra veri türlerinin aynı olup olmadığını da kontrol eder. Örneğin:

```javascript
console.log(1 === '1'); // false
console.log(1 === 1); // true
console.log(0 === false); // false
```

Yukarıdaki örneklerde görüldüğü gibi, `==` operatörü veri türlerini dikkate almadan sadece değerleri karşılaştırırken, `===` operatörü veri türlerini de dikkate alarak karşılaştırma yapar. Bu nedenle, `===` operatörü, daha katı bir eşleşme kontrolü sağlar.

## 10. let var const farkını tablo yapınız

| Özellikler          | let                           | var                       | const                   |
|-------------------|-------------------------------|---------------------------|-------------------------|
| Blok kapsamı       | Evet (sadece blok kapsamında)  | Hayır (fonksiyon kapsamı) | Evet (sadece blok kapsamında)  |
| Tekrar tanımlama   | Evet                          | Evet                      | Hayır                   |
| Tekrar atama       | Evet                          | Evet                      | Hayır                   |
| Oluşturma zamanı   | Çalışma zamanı                | Çalışma zamanı            | Oluşturma zamanı        |
| Hosting            | Hayır (Temporal Dead Zone var) | Evet                      | Hayır                   |

## 11. Arrow fonksiyonun normal fonksiyondan farkları nelerdir
Arrow fonksiyonları (arrow functions) ve normal fonksiyonlar (regular functions), JavaScript'te fonksiyon tanımlamak için kullanılan iki farklı yöntemdir. Arrow fonksiyonları, ES6 (ECMAScript 2015) ile birlikte JavaScript'e eklenen bir özelliktir. İşte bu iki fonksiyon türü arasındaki farklar:

### Arrow Fonksiyonları ve Normal Fonksiyonlar Arasındaki Farklar:

1. **Syntax (Sözdizimi):** Arrow fonksiyonları daha kısa bir sözdizimine sahiptir. 

   Örnek:
   ```javascript
   // Arrow Fonksiyonu
   const func = (param) => { 
       return param; 
   };

   // Normal Fonksiyon
   function func(param) {
       return param;
   }
   ```

2. **`this` Bağlamı:** Arrow fonksiyonları, kendi `this` değerlerini oluşturmaz ve genellikle bulundukları kapsamdaki `this` değerini alırlar. Normal fonksiyonlar ise kendi `this` değerlerini oluştururlar.

3. **Argümanlar (Arguments):** Arrow fonksiyonları, kendi argümanlar objesini oluşturmaz ve `arguments` değişkenine erişemez. Normal fonksiyonlar ise argümanlar objesini oluşturur ve `arguments` değişkenine erişebilir.

4. **Constructor Olarak Kullanım:** Arrow fonksiyonları, constructor olarak kullanılamazlar, yani `new` anahtar kelimesi ile yeni bir örnek oluşturulamazlar. Normal fonksiyonlar ise constructor olarak kullanılabilirler.

5. **Prototip (Prototype) Özelliği:** Arrow fonksiyonları, kendi `prototype` özelliklerine sahip değillerdir. Normal fonksiyonlar ise `prototype` özelliklerine sahiptirler.

6. **İsimlendirme:** Arrow fonksiyonlarının isimlendirme kısıtlamaları vardır ve isimlendirilmiş bir formda kullanılmazlar. Normal fonksiyonlar ise isimlendirilebilirler.

Arrow fonksiyonları, kısa ve anlaşılır bir sözdizimi ile özellikle kısa ve basit fonksiyon tanımlamaları için tercih edilirken, normal fonksiyonlar genellikle daha karmaşık senaryolar için kullanılır.

## 12. swich bloğu içinde hatasız nasıl değişken tanımlanır
Switch bloğu içinde değişken tanımlamak için `let` veya `const` anahtar kelimelerini kullanabilirsiniz. Bununla birlikte, her durumda değişken tanımlamak istiyorsanız, `let` veya `const` anahtar kelimelerini kullanmalısınız. Bunu aşağıdaki gibi yapabilirsiniz:

```javascript
switch (expression) {
  case value1:
    let variable1 = someValue;
    // ...
    break;
  case value2:
    let variable2 = someOtherValue;
    // ...
    break;
  // ...
  default:
    let defaultVariable = defaultValue;
}
```

Bu şekilde, switch durumlarının her biri için kendi kapsamlarında değişken tanımlamış olursunuz. Böylece, her durum için ayrı değişkenler oluşturabilirsiniz ve bu değişkenler sadece kendi kapsamlarında erişilebilir olacaktır. Bu, değişkenlerin farklı durumlar arasında karışmasını önler ve hata ayıklamayı kolaylaştırır.

## 13. Pure fonksiyon ne demektir açıklayınız
Pure fonksiyonlar, programlama terimleri içinde, iki temel özelliğe sahip fonksiyonlardır. Bu özellikler şunlardır:

1. **Yan Etki (Side Effects) Oluşturmama:** Pure fonksiyonlar, programın geri kalanı üzerinde herhangi bir yan etki oluşturmadan, yani dış dünyadaki herhangi bir değişikliği etkilemeden çalışır. Örneğin, dosya okuma veya yazma gibi dış etkileşimler yapmazlar, global değişkenleri değiştirmezler ve herhangi bir veritabanı güncellemesi yapmazlar.

2. **Referans Şeffaflığı (Referential Transparency):** Herhangi bir zamanda ve herhangi bir yerde, aynı girdi (input) değerleriyle çağrıldıklarında her zaman aynı çıktıyı (output) üretirler. Bu, fonksiyonun içinde dışarıdan erişilebilen herhangi bir durum (state) olmaması ve herhangi bir durum değişkenliğine dayanmaması anlamına gelir.

Pure fonksiyonlar, programlama paradigması içinde önemli bir kavramdır. Çünkü bu tür fonksiyonlar, kodun tahmin edilebilirliğini artırır, hata ayıklamayı kolaylaştırır, test edilebilirliği artırır ve kodun okunabilirliğini artırır. Bu nedenle, mümkün olduğunca birçok pure fonksiyon kullanmak genellikle tercih edilir.

Örnek bir pure fonksiyon:

```javascript
function multiplyByTwo(x) {
  return x * 2;
}
```

Bu fonksiyon, herhangi bir dış etki oluşturmadan ve herhangi bir dış duruma dayanmadan her zaman aynı girdi değeriyle aynı çıktıyı üretir.

## 14. Rest operatör nedir örnekle açıklayınız
Rest operatörü, fonksiyonlara veya dizi ve nesne gibi veri yapılarına dinamik sayıda argüman veya öğe geçirilmesini sağlayan bir JavaScript operatörüdür. Bu operatör, üç nokta (`...`) karakteri ile gösterilir. Fonksiyonlarda rest parametresi olarak kullanıldığında fonksiyona geçilen tüm argümanları bir dizi olarak toplar. Dizi veya nesnelerde kullanıldığında ise öğeleri ayrı ayrı alır.

### Fonksiyonlarda Rest Parametresi Örneği:

```javascript
function sum(...numbers) {
  return numbers.reduce((acc, val) => acc + val, 0);
}

console.log(sum(1, 2, 3, 4, 5)); // 15
```

Yukarıdaki örnekte, `sum` fonksiyonu rest parametresi `...numbers` ile bir dizi olarak tüm geçilen argümanları toplar.

### Dizi Kopyalama veya Birleştirme Örneği:

```javascript
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];

const combinedArray = [...array1, ...array2];
console.log(combinedArray); // [1, 2, 3, 4, 5, 6]
```

Yukarıdaki örnekte, `...array1` ve `...array2` rest operatörü ile ayrı ayrı öğeleri alınarak `combinedArray` adlı yeni bir dizi oluşturulur.

Rest operatörü, kodun okunabilirliğini artırır ve dinamik sayıda argümanların veya öğelerin işlenmesini kolaylaştırır. Bu nedenle, genellikle fonksiyonlarda veya dizilerde ve nesnelerde veri işleme süreçlerinde kullanılır.

## 15. Object destructuring nedir örnekle açıklayınız


Object destructuring, bir nesnenin özelliklerini ayrıştırarak, bu özelliklere erişimi kolaylaştıran bir JavaScript özelliğidir. Bu işlem, nesne içindeki belirli özelliklere erişmek için kullanılır. Nesne destructuring sürecinde, nesne özellikleri, değişkenlere atanabilir veya farklı değişken isimleri kullanılarak değişkenlere atama yapılabilir.

### Nesne Destructuring Örneği:

```javascript
const person = { 
  name: 'John', 
  age: 30, 
  country: 'USA' 
};

// Destructuring ile özelliklere erişim
const { name, age, country } = person;

console.log(name); // John
console.log(age); // 30
console.log(country); // USA
```

Yukarıdaki örnekte, `person` nesnesinin özelliklerine, `name`, `age` ve `country` değişkenleri üzerinden erişim sağlanır.

### Farklı Değişken İsimleri ile Nesne Destructuring Örneği:

```javascript
const person = { 
  name: 'John', 
  age: 30, 
  country: 'USA' 
};

// Farklı değişken isimleriyle destructuring
const { name: personName, age: personAge, country: personCountry } = person;

console.log(personName); // John
console.log(personAge); // 30
console.log(personCountry); // USA
```

Yukarıdaki örnekte, `person` nesnesinin özelliklerine `personName`, `personAge` ve `personCountry` değişkenleri üzerinden erişim sağlanır.

Object destructuring, karmaşık nesnelerin içindeki verilere erişimi kolaylaştırır ve daha temiz, daha okunabilir kod yazmanıza yardımcı olur. Bu nedenle, özellikle API cevapları gibi karmaşık nesnelerle çalışırken sıkça kullanılır.

## 16. 2 elemanlı bir objeyi 6 farklı şekilde oluşturunuz
İki elemanlı bir objeyi JavaScript'te altı farklı şekilde oluşturmak mümkündür. İşte bu altı farklı yöntem:

1. **Objeleri Elle Oluşturma:**
```javascript
const obj1 = { key1: 'value1', key2: 'value2' };
```

2. **Object Constructor Yöntemiyle Oluşturma:**
```javascript
const obj2 = new Object();
obj2.key1 = 'value1';
obj2.key2 = 'value2';
```

3. **Object.create Yöntemiyle Oluşturma:**
```javascript
const obj3 = Object.create(null);
obj3.key1 = 'value1';
obj3.key2 = 'value2';
```

4. **Kısa İfadelerle Oluşturma:**
```javascript
const key1 = 'value1';
const key2 = 'value2';
const obj4 = { key1, key2 };
```

5. **Değişkenlerle Oluşturma:**
```javascript
const key1 = 'value1';
const key2 = 'value2';
const obj5 = {};
obj5[key1] = key1;
obj5[key2] = key2;
```

6. **Array Destructuring Yöntemiyle Oluşturma:**
```javascript
const [key1, key2] = ['value1', 'value2'];
const obj6 = { key1, key2 };
```

Bu örneklerle, iki elemanlı bir objenin farklı şekillerde nasıl oluşturulabileceğini göstermiş olduk. Bu farklı yöntemler, programlama stilinize ve kullanım durumunuza göre değişebilir.

## 17. 2 elemanlı bir objenin key ve value değerlerinin karakter sayısı ile 2 farklı döngü methodu kullanarak yeni bir obje oluşturunuz
// İlk olarak, verilen 2 elemanlı objeyi oluşturalım
const obj = { key1: 'value1', key2: 'value2' };

// Method 1: for...in döngüsü kullanarak yeni bir obje oluşturma
let newObj1 = {};
for (let key in obj) {
    let length = key.length + obj[key].length;
    newObj1[key] = length;
}
console.log("Yeni obje (for...in):", newObj1);

// Method 2: Object.entries() ve Array.prototype.forEach() kullanarak yeni bir obje oluşturma
let newObj2 = {};
Object.entries(obj).forEach(([key, value]) => {
    let length = key.length + value.length;
    newObj2[key] = length;
});
console.log("Yeni obje (Object.entries()):", newObj2);

## 18. Cookie, local storage ve session storage farkını tablo yapınız

| Özellikler          | Cookie                                    | Local Storage                            | Session Storage                      |
|-------------------|-------------------------------------------|------------------------------------------|--------------------------------------|
| Veri saklama      | 4KB'a kadar veri saklayabilir.            | 5MB'a kadar veri saklayabilir.            | 5MB'a kadar veri saklayabilir.         |
| Tarayıcıya gönderme | HTTP isteklerinde otomatik olarak gönderilir. | Manuel olarak JavaScript kullanılarak gönderilir. | Oturum sona erdiğinde silinir.      |
| Kullanım amacı     | Oturum yönetimi, kimlik doğrulama vb.       | Kalıcı veri depolama, yerel veriler.       | Oturum verilerini geçici olarak saklama. |
| Süresi            | Belirlenen bir süreye veya tarayıcı kapatılana kadar kalabilir. | Kalıcıdır, veri silinene kadar kalır.      | Tarayıcı oturumu boyunca kalır, oturum sona erdiğinde silinir. |

## 19. asenkron ve senkron işlem farkı nedir
Senkron işlemler, bir önceki işlem tamamlanmadan bir sonraki işleme geçmeyi bekler. Bu nedenle, işlemler sıralı ve bekleyerek gerçekleşir. Öte yandan, asenkron işlemler, bir işlemin tamamlanmasını beklemeden diğer işlemleri yürütebilir. Bu özellikle uzun sürecek işlemler, ağ istekleri veya dosya okuma/yazma gibi giriş/çıkış işlemlerinde faydalıdır. Asenkron işlemler genellikle non-blocking olarak adlandırılır, çünkü bir işlemin tamamlanmasını beklemeksizin diğer işlemler devam edebilir. Bu da genellikle uygulamanın daha hızlı ve verimli çalışmasına yardımcı olabilir.

## 20. promise nedir ve neden ihtiyaç duyarız
Promise, JavaScript'te asenkron programlama yaparken kullanılan bir nesnedir. Asenkron işlemler, belirli bir işlem tamamlanana kadar diğer işlemlerin devam etmesini sağlar. Promise, asenkron işlemler için bir sonuç veya hata döndürme mekanizması sağlar ve işlemin tamamlanıp tamamlanmadığını izlemek için kullanılır.

Promise yapısı, resolve, reject ve finally olmak üzere üç farklı yöntem sunar. Bu yöntemler, Promise nesnesinin durumunu ve sonucunu belirlemek için kullanılır:

Promise'ler, callback fonksiyonlarının ve callback cehennemi olarak adlandırılan kod karmaşıklığını azaltmaya yardımcı olur. Birden fazla asenkron işlem birbirini takip ediyorsa veya birleştiriliyorsa, kodunuzun okunabilirliğini ve bakımını kolaylaştırır.

Promise'ler ayrıca ağ istekleri, dosya okuma/yazma işlemleri, zamanlayıcılar gibi asenkron işlemler için kullanılır. Bu tür durumlarda, işlemin tamamlanmasını beklemek ve sonucunu veya hata durumunu ele almak için promise'ler kullanılır.

Sonuç olarak, Promise'ler JavaScript'te asenkron programlama yaparken, kodun daha okunabilir, yönetilebilir ve hatasız olmasını sağlayan önemli bir yapısal bileşendir.


# Array Soruları
# var dolap = ["Shirt", "Pant", "TShirt"];
## 1. dolap arrayindeki son elemanı silip consola yazdırın
```javascript
dolap.pop(); // Son elemanı silme
console.log(dolap); // Konsola yazdırma
```

## 2. dolap arrayindeki ilk elamanı silip yerine “Hat” elemanını gönderip consola yazdırın
```javascript
dolap.shift(); // İlk elemanı silme
dolap.unshift("Hat"); // "Hat" elemanını başa ekleme
console.log(dolap); // Konsola yazdırma
```

## 3. dolap değişkeninin array olup olmadığını kontrol edin ve sonucu bir değişkene eşitleyin
```javascript
let isArray = Array.isArray(dolap); // Array olup olmadığını kontrol etme
```

## 4. dolap arrayinde “Pant” elemanın olup olmadığını 3 farklı method ile kontrol edin
```javascript
let check1 = dolap.includes("Pant"); // includes() yöntemi
let check2 = dolap.indexOf("Pant") !== -1; // indexOf() yöntemi
let check3 = dolap.find((element) => element === "Pant"); // find() yöntemi
```

## 5. dolap arrayindeki elemanların karakter sayısını toplayıp geriye döndürecek fonksiyonu yazın
```javascript
function toplamKarakterSayisi(arr) {
  let toplam = 0;
  for (let i = 0; i < arr.length; i++) {
    toplam += arr[i].length;
  }
  return toplam;
}

let karakterToplami = toplamKarakterSayisi(dolap); // Fonksiyonu çağırma
```

## 6. dolap arrayindki tüm elemanları büyük harfe çevirip yeni bir değişkene 3 farklı yöntemle atayın
```javascript
let buyukHarfDolap1 = dolap.map((item) => item.toUpperCase()); // map() ve toUpperCase() yöntemi
let buyukHarfDolap2 = dolap.join(" ").toUpperCase().split(" "); // join(), toUpperCase() ve split() yöntemi
let buyukHarfDolap3 = dolap.reduce((acc, curr) => [...acc, curr.toUpperCase()], []); // reduce() ve toUpperCase() yöntemi
```

## 7. dolap arrayini index sayıları key olacak şekilde objeye çeviriniz
```javascript
let objeDolap = {};
dolap.forEach((element, index) => {
  objeDolap[index] = element;
});
```

## 8. slice ile splice farkı nedir
- `slice`: Bir dizinin belirli bir bölümünü kopyalar ve bu kısmı yeni bir dizi olarak döndürür. Orijinal dizi üzerinde herhangi bir değişiklik yapmaz.
- `splice`: Bir dizide belirtilen konumdan itibaren belirli bir sayıda öğeyi kaldırır ve isteğe bağlı olarak yeni öğeler ekler. Orijinal dizi üzerinde değişiklik yapar.

# const arr = [1,2,3,4,5,6,7,7,8,6,10];
## 1. arrayindeki yinelenen sayıları bulun
```javascript
const yinelenenler = arr.filter((item, index) => arr.indexOf(item) !== index);
```

## 2. arrayindeki tüm yinelenen sayıları silip yeni bir arrayi 2 farklı method ile oluşturun 
```javascript
const uniqueArray1 = arr.filter((item, index) => arr.indexOf(item) === index);
const uniqueSet = new Set(arr);
const uniqueArray2 = [...uniqueSet];
```

## 3. arrayindeki en yüksek ve en düşük değeri 2 farklı methodla bulun
```javascript
const enYuksek1 = Math.max(...arr);
const enDusuk1 = Math.min(...arr);

const enYuksek2 = arr.reduce((a, b) => Math.max(a, b));
const enDusuk2 = arr.reduce((a, b) => Math.min(a, b));
```
# Kod Çıktı Soruları
```javascript
// Bu kodun çıktısı nedir neden ?
function job() {
    return new Promise(function(resolve, reject) {
        reject();
}); }
let promise = job();
promise
.then(function() {
    console.log('Success 1');
})
.then(function() {
    console.log('Success 2');
})
.then(function() {
    console.log('Success 3');
})
.catch(function() {
    console.log('Error 1');
})
.then(function() {
    console.log('Success 4');
});
```
Bu kodun çıktısı aşağıdaki gibi olacaktır:

```
Error 1
Success 4
```
Kodun akışını incelediğimizde, job fonksiyonu bir Promise döndürür ve bu Promise bir reject ile sonuçlanır. Dolayısıyla, catch bloğu çalışır ve 'Error 1' yazdırılır.

Daha sonra, bir dizi ardışık then fonksiyonu gelir. Ancak, catch bloğu çalıştıktan sonra bile, bu then fonksiyonları zincirin geri kalanını başarılı kabul eder. Bu nedenle, 'Success 4' yazdırılır.

Sonuç olarak, çıktı "Error 1" ve "Success 4" olacaktır. Bu, catch bloğunun işleyişini ve ardından gelen then bloklarının nasıl çalıştığını göstermektedir.

```javascript
// Bu kodun çıktısı nedir neden ?
function job(state) {
    return new Promise(function(resolve, reject) {
        if (state) {
            resolve('success');
        } else {
            reject('error');
        }
}); }
let promise = job(true);
promise
.then(function(data) {
    console.log(data);
    return job(true);
})
.then(function(data) {
    if (data !== 'victory') {
        throw 'Defeat';
    }
    return job(true);
})
.then(function(data) {
    console.log(data);
})
.catch(function(error) {
    console.log(error);
    return job(false);
})
.then(function(data) {

console.log(data);
    return job(true);
})
.catch(function(error) {
    console.log(error);
    return 'Error caught';
})
.then(function(data) {
    console.log(data);
    return new Error('test');
})
.then(function(data) {
    console.log('Success:', data.message);
})
.catch(function(data) {
    console.log('Error:', data.message);
});
```

Bu kod parçasının çıktısı aşağıdaki gibi olacaktır:

```
success
Defeat
error
Error caught
Success: test
```

Kodun akışını incelediğimizde:

1. `job(true)` çağrısı, ilk `then` bloğuna bir 'success' değeri döndürür.
2. İkinci `then` bloğu, 'victory' olmadığı için bir 'Defeat' hatası fırlatır ve `catch` bloğuna yönlendirilir.
3. `catch` bloğu, 'error' yazdırır ve bir sonraki `then` bloğuna 'false' durumu ile yönlendirilir.
4. Sonraki `then` bloğu, 'success' yazdırır.
5. Sonraki `catch` bloğu, 'error' yazdırır ve 'Error caught' döndürür.
6. Dördüncü `then` bloğu, bir hata nesnesi oluşturur, bu obje `then` bloğuna gider ve 'Succcess: test' yazdırılır.

