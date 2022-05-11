# PyScript Türkçe Dökümantasyon

Başlamadan önce: kaynağa destek olabilir ve daha çok kişiye erişmesini sağlayabilirsiniz. 🎉⭐

## PyScript nedir?
Anaconda'dan Peter Wang, Fabio Pliger ve Philipp Rudiger'in içerisinde bulunduğu  bir ekip tarafından geliştirilen PyScript, Peter'ın konuşmasında belirttiği gibi, Python'u PHP gibi HTML içerisinde yazabilmek için geliştirilen bir JavaScript framework'üdür.Bu, Python kodunu HTML dosyasının içerisinde yazıp çalıştırabileceğiniz anlamına gelir.Sizcede kulağa müthiş gelmiyor mu :)

### PyScript'i kullanmak dünya ve veri bilimcileri için ne anlama geliyor?
En belirgin şey, PyScript ile artık Python'u (ve potansiyel olarak diğer dilleri) HTML'de yazabiliyor ve web uygulamaları oluşturabiliyoruz. PyScript, Python'un gücünü front-end kısmındaki geliştiriciler için erişilebilir kılar.

Peter'ın konuşmada belirttiği gibi, "web tarayıcısı dünyanın en yaygın, taşınabilir bilgisayar ortamıdır." Gerçekten de, ister bilgisayarda ister telefonda olsun, hemen hemen herkesin bir web tarayıcısına erişimi vardır. Bu, herhangi bir altyapı engeli olmaksızın herkesin erişebileceği ve programlamaya başlayabileceği anlamına gelir.
Her şey web tarayıcınızda gerçekleşecek. Veri bilimcileri olarak, panolarımızı ve modellerimizi, başkaları dosyayı bir web tarayıcısında açtığında kodu çalıştıracak bir html dosyasında paylaşabiliriz.

### PyScript'in arkasındaki sihir nedir?
PyScript şu anda "CPython'dan WebAssembly/Emscripten" 'a port olan Pyodide üzerine kuruludur. PyScript, bir tarayıcıda Python kodu yazmayı ve çalıştırmayı destekler ve gelecekte diğer diller için destek sağlayacaktır.

![İşleyiş Resmi](https://anaconda.cloud/api/files/31ea07ba-dadc-4d18-b79e-d309328762d0)

### WebAssembly nedir?
Python'da web siteleri yazmayı mümkün kılan temel teknoloji WebAssembly'dir. WebAssembly ilk geliştirildiğinde, web tarayıcıları yalnızca Javascript'i destekliyordu.

İlk olarak 2017'de piyasaya sürülen WebAssembly, 2019'a kadar hızla resmi World Wide Web Consortium (W3C) standardı haline geldi. İnsanlar tarafından okunabilen bir .wat  formatında dosya içerir ve bu dosya daha sonra tarayıcıların çalıştırabileceği bir binary (ikili) .wasm formatına dönüştürülür. Bu, herhangi bir dilde kod yazmamızı, onu WebAssembly'de derlememizi ve ardından bir web tarayıcısında çalıştırmamızı sağlar.


### PyScript nasıl kullanılır?
PyScript'in alfa sürümüne [buraya](pyscript.net) tıklayarak ulaşabilirsiniz. Kodları https://github.com/pyscript adresinde mevcuttur. Denemek için bu talimatları izleyin. PyScript, aşağıdaki üç ana bileşeni kullanarak Python'u html'de yazmanıza izin verir:



1.py-env, Python kodunuzu çalıştırmak için gereken Python paketlerini tanımlar.

2.py-script, web sayfasında çalıştırılan Python kodunuzu yazdığınız yerdir.

3.py-repl, kullanıcıların girdiği kodu değerlendiren ve sonuçları görüntüleyen bir REPL (okuma-değerlendirme-yazdırma döngüsü) bileşeni oluşturur.


### py-env örneği
Python ortamımızı py-env kullanarak bir HTML'de nasıl tanımlayabileceğimize dair bir örnek. Bu örnekte, bokeh, numpy, pandas ve scikit-learn paketlerini ortamımıza yüklüyoruz.

![py-env](https://anaconda.cloud/api/files/803653a5-9b1e-41d4-a9ee-76c64b8d6cb4)


### py-script örneği
Bu örnek, akış verileri içeren bir Panel panosunu gösterir. Kodda da görebileceğiniz gibi, normalde bir Python dosyasında yaptığımız gibi, Python kodumuzu py-script'e yazabiliyoruz. Python kodunuzu doğrudan py-script taglarının içine yazmayı sevmiyorsanız, kaynak kodu olarak bir Python dosyası da kullanabilirsiniz:

`<py-script>Python Kodları</py-script>` örneğin 
`<py-script> 
      print("Hello PyScript!")
</py-script>`

ya da bu şekilde kullanabilirsiniz:

![py-script](https://anaconda.cloud/api/files/c57a6ef0-dbb7-43da-acd9-94a781ef2673)

![py-script](https://anaconda.cloud/api/files/27806bdc-84f8-40a2-baf3-da1b08ea5f1c)


### py-repl örneği

Bu örnek, DeckGL ve REPL bileşenini kullanan NYC Taksi verileriyle bir Panel panosunu gösterir. Gördüğünüz gibi, REPL'de yarıçapı tanımlayabiliyor ve data framework'ünün (hour<3) subset'ini seçebiliyoruz.

![py-script](https://anaconda.cloud/api/files/94b36d4e-a856-4c53-b3b1-1055ef7f582a)




Ayrıca, [buraya](https://github.com/pyscript) tıklayarak, 3 boyutlu ve bilgisayar görüşüne sahip bir Mario oyunu da dahil olmak üzere birçok başka örnek bulabilirsiniz.


## Kaynakça
https://www.anaconda.com/


