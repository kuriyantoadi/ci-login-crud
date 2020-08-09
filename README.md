# CodeIgniter-Login-Bootstrap-CRUD

**1. Extrak Framework CI**

**2. Import database db-buku.sql**

**3. application/config/autoload.php**
  <br>Awal Baris 92 :
  <br>`$autoload['helper'] = array('');`
  <br>Edit :
  <br>`$autoload['helper'] = array('url','form');`

  <br>Awal Baris 61 :
  <br>`  $autoload['libraries'] = array('');`
  <br>Edit :
  <br>`  $autoload['libraries'] = array('database');`

  **4. application/config/database.php ubah baris 78-81**
  <br>`'hostname' => 'localhost',`
  <br>`'username' => 'root',`
  <br>`'password' => '',`
  <br>`'database' => 'db_buku',`

  **5. application/config/config.php ubdah baris 26**
  <br>`$config['base_url'] = '';`
  <br>Edit
  <br>Alamat disesuaikan dengan nama project
  <br>`$config['base_url'] = 'http://localhost/ci-login-crud/';`

  **6. Tambah folder asset**
  <br>Folder ini berisi file bootstrap dan js

  **7. Tambahkan/Edit beberapa file berikut**
  - application/controllers/C_buku.php -> Controller untuk tambah, tampil, edit dan hapus buku
  - application/controllers/C_login.php -> Controller untuk login user
  - application/controllers/C_page.php -> Controller untuk mengarahkan ke View Tampil buku
  - application/models/M_buku.php -> Menghubukan controller dengan Database Data Buku
  - application/models/M_login.php -> Menghubukan controller dengan Database Login User
  - application/view/buku/v_edit.php -> File untuk edit data buku
  - application/view/buku/v_tambah.php -> File untuk tambah data buku
  - application/view/buku/v_tampil.php -> File untuk tampil data buku


  **8. application/config/routes.php ubah baris 52**
  <br>`$route['default_controller'] = 'C_buku';`

  **9. Buka dengan Link berikut**
  <br>`localhost/ci-bootstrap-crud`

  (catatan ini adalah lanjutan dari repository ci-crud-tambah)
