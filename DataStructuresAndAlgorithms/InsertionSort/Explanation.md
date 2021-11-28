# Project 1 (Insertion Sort)

> Array -> [22, 27, 16, 2, 18, 6]

<br>

![UNSORTED-ARRAY](Documents/Images/UnsortedArray.png?raw=true)

<br>

## 1) **EN**: Please write the above array sorting steps by using insertion sort. (**TR**: Yukarıda verilen dizinin sıralama aşamalarını insertion sort'a göre yazınız.)

<br>

---

<br>

1. **[22, 27, 16, 2, 18, 6]**
   - **_EN_**: In this section, firstly we picked up 27 and we compared them with 22. 27 is bigger than 22 so, our first 2 element of the array anyway sorted in beginning.
     <br>
     <br>
   - **_TR_**: Bu aşamada ilk olarak 27'yi seçtik ve onu 22 ile karşılaştırdık. 27, 22'den büyüktür böylece bizim dizimizin ilk 2 elemanı zaten başlangıçta sıralanmıştır.

<br>

![STEP-1-RESULT-ARRAY](Documents/Images/STEP%201.png?raw=true)

<br>

2. **[16, 22, 27, 2, 18, 6]**
   - **_EN_**: After the two elements of array (22 and 27), we picked the third element, its 16! And we began comparing 16 with sorted values. (again 22 and 27). When we start compare a number with others we need to know we are moving left one by one. So our first comparison is 16 and 27 (If you confuse about this, you can look the array of on first step header.). Is 27 smaller than 16 ? Its not. So we need move 16 to left side of 27 and now our array look like this: [22, 16, 27, 2, 18, 6]. But our process still continue. Look the first three value of array. There are 22, 16 and 27. This place our sorted area but if you look carefully 16 smaller than 22, end of the process we need to have smallest value at the first index of array so we moved the value 16 again. Now looks well! ([16, 22, 27, 2, 18, 6])
     <br>
     <br>
   - **_TR_**: Dizinin iki elemanından sonra (22 ve 27) 3. elemanı seçtik, 16'yı! ve 16'yı sıralanmış değerlerle (tekrar 22 ve 27) karşılaştırmaya başladık. Bir sayıyı bir başka sayıyla karşılaştırmaya başladığımızda bilmemiz gereken hareket yönümüzün birer birer ve sola doğru olduğudur yani ilk karşılaştırmamız 16 ve 27'dir (Eğer aklınız karıştıysa ilk adımın başlığındaki diziye bakabilirsiniz.). 27, 16'dan küçük mü ? Hayır değil böylelikle 16'yı 27'nin sol tarafına hareket ettirdik ve dizimiz şu an böyle gözüküyor: [22, 16, 27, 2, 18, 6] ama bizim işlemimiz hala devam ediyor. Dizinin ilk 3 değerine bakın. 22, 16 ve 27 var. Bu yer bizim sıralanmış alanımız ama eğer dikkatlice bakarsanız 16, 22'den küçüktür. İşlemin sonunda en küçük değerin, dizinin ilk sırasında olması gerekir böylece biz 16'yı tekrar hareket ettirdik ve şu an dizimiz güzel gözüküyor! ([16, 22, 27, 2, 18, 6])

<br>

![STEP-2-RESULT-ARRAY](Documents/Images/STEP%202.png?raw=true)

<br>

3. **[2, 16, 22, 27, 18, 6]**
   - **_EN_**: We are going to repeat same process. The main objective is, pick an element from the array and start compare that element left by left until encounter the smaller than our picked element. Turn is at fourth element of array. That element is 2. Our array looks like this now: [16, 22, 27, 2, 18, 6]. Pick the fourth element (2) and start compare this element left by left. Is 27 smaller than 2 ? No so we changed positions these elements. Array looks like this now: [16, 22, 2, 27, 18, 6]. Lets repeat process. Is 22 smaller than 2 ? No, so we changed positions again. One more process for finish step 3, and our array looks like this: [16, 2, 22, 27, 18, 6]. Is 16 smaller than 2 ? No, so we changed positions again and looks well! [2, 16, 22, 27, 18, 6]
     <br>
     <br>
   - **_TR_**: Aynı işlemi tekrar edeceğiz. Asıl amacımız dizimizden bir eleman seçip onu dizi içinde sola doğru kendisinden daha küçük bir elemanla karşılaşana kadar karşılaştırmaktır. Sıra dizinin dördüncü elemanında. Bu eleman 2'dir. Şu an dizimiz bu şekilde gözüküyor: [16, 22, 27, 2, 18, 6]. Dördüncü elemanı seçin (2) ve bu elemanı sola doğru karşılaştırmaya başlayın. 27, 2'den küçük mü ? Hayır bu yüzden bu elemanların dizi içerisindeki pozisyonlarını değiştirdik. Dizi şu an bu şekilde gözüküyor: [16, 22, 2, 27, 18, 6]. İşlemi tekrar edelim. 22, 2'den küçük mü ? Hayır bu yüzden yerlerini değiştirdik. Adım üçün bitmesi için son bir işlem kaldı ve bizim dizimiz şu an böyle gözüküyor: [16, 2, 22, 27, 18, 6]. 16, 2'den küçük mü ? Hayır bu yüzden tekrar yerlerini değiştirdik ve şu an güzel gözüküyor! [2, 16, 22, 27, 18, 6]

<br>

![STEP-3-RESULT-ARRAY](Documents/Images/STEP%203.png?raw=true)

<br>

4. **[2, 16, 18, 22, 27, 6]**
   - **_EN_**: Our array looks like this: [2, 16, 22, 27, 18, 6]. And turn is at fifth element (18). Lets look array. [2, 16, 22, 27] there is a sorted area, however [18, 6] not sorted now lets begin with 18, the array fifth element. Is 27 smaller than 18 ? No, so we changed positions. Array looks like this now: [2, 16, 22, 18, 27, 6]. Is 22 smaller than 18 ? No, so we changed positions again and array looks like this now: [2, 16, 18, 22, 27, 6]. Is 16 smaller than 22 ? Yes, so our fourth step is over. Array is sorted for fifth element but we have one more element.
     <br>
     <br>
   - **_TR_**: Bizim dizimiz şu an böyle gözüküyor: [2, 16, 22, 27, 18, 6] ve sıra beşinci elemanda (18). Dizimize bakalım. [2, 16, 22, 27] burada sıralanmış alan var ama [18, 6] sıralanmamıştır, şimdi dizinin beşinci elemanı olan 18 ile başlayalım. 27, 18'den küçük mü ? Hayır bu yüzden yerlerini değiştirdik. Dizi şu an bu şekilde gözüküyor: [2, 16, 22, 18, 27, 6]. 22, 18'den küçük mü ? Hayır böylece yerlerini tekrar değiştirdik ve dizimiz şu an bu şekilde gözüküyor: [2, 16, 18, 22, 27, 6]. 16, 22'den küçük mü ? Evet böylece bizim dördüncü adımımız bitti. Dizi beşinci eleman için de sıralandı ama bir elemanımız daha var.

<br>

![STEP-4-RESULT-ARRAY](Documents/Images/STEP%204.png?raw=true)

<br>

5. **[2, 6, 16, 18, 22, 27]**
   - **_EN_**: We came the last step of sorting array with insertion sort. Let's dive into it. Our array looks like this: [2, 16, 18, 22, 27, 6]. Lets pick sixth element of array (6). Is 27 smaller than 6 ? No, we changed positions and array looks like this: [2, 16, 18, 22, 6, 27]. Is 22 smaller than 6 ? No, we changed positions, here is the array: [2, 16, 18, 6, 22, 27]. Is 18 smaller than 6 ? No, we changed positions and there is a new array: [2, 16, 6, 18, 22, 27]. Is 16 smaller than 6 ? No, lets change the positions [2, 6, 16, 18, 22, 27]. And the final step: Is 2 smaller than 6 ? Yes. So we finished the sorting array with insertion sort.
     <br>
     <br>
   - **_TR_**: Eklemeli sıralama (insertion sort) ile dizimizi sıralamada son adıma geldik. Hadi şunu yapalım. Dizimiz bu şekilde gözüküyor: [2, 16, 18, 22, 27, 6]. Dizinin altıncı elemanını seçelim (6). 27, 6'dan küçük mü ? Hayır bu yüzden yerlerini değiştirdik ve dizimiz bu şekilde gözüküyor: [2, 16, 18, 22, 6, 27]. 22, 6'dan küçük mü ? Hayır, yerlerini değiştirdik, dizimiz burada: [2, 16, 18, 6, 22, 27]. 18, 6'dan küçük mü ? Hayır, yerlerini değiştirdik ve yeni bir dizimiz var: [2, 16, 6, 18, 22, 27]. 16, 6'dan küçük mü ? Hayır, hadi yerlerini değiştirelim [2, 6, 16, 18, 22, 27] ve son adıma geldik: 2, 6'dan küçük mü ? Evet. Böylece dizimizi eklemeli sıralama (insertion sort) ile sıralamayı bitirdik.

<br>

![STEP-5-RESULT-ARRAY](Documents/Images/STEP%205.png?raw=true)

<br>

> EN: **Sorted array with _Insertion Sort_**: `[2, 6, 16, 18, 22, 27] (NOT sorted: [22, 27, 16, 2, 18, 6])` > <br>
> TR: **_Insertion Sort (Eklemeli sıralama)_ ile sıralanmış dizi** : `[2, 6, 16, 18, 22, 27] (SIRALANMAMIŞ: [22, 27, 16, 2, 18, 6])`

<br>

![SORTED-ARRAY](Documents/Images/SortedArray.png?raw=true)

<br>
