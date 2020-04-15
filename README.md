
# minggu-7
* $data = $hasil->fetch(PDO::FETCH_ASSOC); : merubah data yang
  dieksekusi ke dalam bentuk array

* ob_start(); : fungsi ini digunakan sebagai awal untuk menyimpan
  sementara hasil buffer pada php

* $data = $hasil->fetch(PDO::FETCH_OBJ); : fungsi ini digunakan untuk
  merubah data query yang dieksekusi menjadi Object

* $html = ob_get_clean(); : fungsi ini digunakan sebagai akhir untuk
  menyimpan hasil buffer pada php kemudian disimpan ke $html

* $dompdf = new Dompdf\Dompdf(); : fungsi OOP untuk memanggil class
  Dompdf

* $dompdf->loadHtml($html); : memasukkan $html untuk dijadikan
  tampilan PDF

* $dompdf->setPaper('A4', 'landscape'); : mengatur ukuran kertas A4
Landscape

* $dompdf->render(); : melakukan rendering tampilan PDF
* $pdf = $dompdf->output(); : menyimpan file PDF sementara ke temporary
  file
* $dompdf->stream('laporan.pdf',array('Attachment' => 0)); : menampilkan
  hasil pdf dengan nama laporan.pdf dan parameter kedua yaitu array
  Attachment, apabila 0 maka hanya tampil di browser dan jika 1 maka
  akan dilakukan proses download


