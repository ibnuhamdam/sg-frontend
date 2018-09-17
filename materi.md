# 1. Manipulasi DOM

A. Mengakses Elemen pada DOM
Sebelum mulai melakukan manipulasi pada elemen DOM, kita harus memilih mana elemen yang akan kita ubah propertinya. ada beberapa fungsi umum yg bisa digunakan untuk akses elemen DOM:

- document.getElementById = Mengakses elemen DOM berdasarkan id nya
- document.getElementsByClassName = Berdasarkan nama class
- document.getElementsByTagName = Berdasarkan Tag nya
- document.querySelector = Mencari elemen DOM pertama yang sesuai dengan aturan selector CSS 
- document.querySelectorAll = Sama seperti querySelector tapi ini mengembalikan semua elemen  (bukan hanya yang pertama saja) 

B. Membuat sebuah elemen DOM
DOM memiliki dua jenis elemen, yaitu elemen node dan teks. Membuat elemen baru untuk DOM juga dilakukan dengan dua cara: document.createElement untuk pembuatan node dan document.createTextNode untuk pembuatan teks.

C. Menghapus Elemen dengan DOM
Penghapusan elemen DOM dilakukan hanya melalui satu fungsi: removeChild. Prosesnya nya: pilih elemen yang akan dihapus, kemudian panggil method removeChild pada penampung elemen yang akan dihapus tersebut.

D. Modifikasi Attribut DOM
Untuk modifikasi attribut pada dom digunakan fungsi: setAttribute('parameter-1: attribut nya', 'param-2: nilainya')
dan untuk hapus attribut yg sudah ada digunakan fungsi: removeAttribute('param-1: attrbute yg ingin dihapus')


# 2. Menganti Tampilan Elemen DOM 

A. Bagian sebelumnya kita sudah belajar bagaimana mengganti atribut elemen DOM, bagian ini  belajar tentang cara menggantikan atribut CSS pada elemen DOM, dengan memanfaatkan attribute *syle* pada sebuh element.

B. Atau dengan langsung mengubah elemen css nya dengan bantuan: classlist
Dengan menggunakan fitur yang disediakan oleh classList ini, kita dapat mengubah tampilan dari sebuah elemen DOM dengan mudah dan rapi.


# 3. DOM Events

Untuk mendapatkan web yang lebih interkatif maka kita perlu sebuah dom events, misalnya saja ketika user menekan sebuah button maka akan memberikan sebuah response ke pengguna, yang mana ini akan lebih bagus untuk pengalaman yg membuka web kita.

A. Cara Listen sebuah events
 - Event Handler
 - Dengan addEventListener(kelebihan bisa menghandle lebih dari satu event sekaligus)

B. Browser DOM Events
 - onclick
 - onkeyup
 - onchange
 - onmouseover
 - dll
   Cek Lengkapnya: https://developer.mozilla.org/en-US/docs/Web/Events


# 4. Menelusuri Element DOM Traversal

Untuk menelusuri DOM: Pertama seleksi elemen menggunakan dom method terlebih dahulu, setelah elemen nya ketemu, kita akan pilih elemen lain yg kita inginkan itu berdasakran elemen yg sudah kita dapat/seleksi tadi.
*Intinya: Untuk mendapatkan sebuh elemen berdasakran elemen yg sudah kita seleksi di awal.

A. Contoh sederhan DOM traversal
Contoh sederhana menggunakan dom traversal.

B. Menggunakan Event Delegation 
Idenya adalah ketika kita punya banyak element yg pengen dihandle pake cara yg sama , daripada kita kasih nilai handler yg sama ke tiap element, lebih baik kita punya satu handle kusus aja buat handle semua nya, jadi lebih bagus dan efisien.

C. Event Prevent Default
Untuk mencegah event atau kelakuan default dari sebuah element.

D. Method yang umum digunakan pada DOM traversal
  - parentElement
  - parentNode
  - nextElementSibling
  - previousElementSibling
  - dll
