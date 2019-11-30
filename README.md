# CodeIgniter-Boostrap
Menghubungkan CI dan Boostrap

**1. Extrak Framework CI dan Boostrap**

**2. application/config/config.php baris 26**
  <br>Awal :
  <br>`$config['base_url'] = '';`
  <br>Edit :
  <br>`$config['base_url'] = 'http://localhost/ci-boostrap';`

**3. application/config/autoload.php baris 92**
  <br>Awal :
  <br>`$autoload['helper'] = array('');`
  <br>Edit :
  <br>`autoload['helper'] = array('url');`
  
**4. application/view/welcome_message.php ganti semua ini dengan syntax berikut**
    <br>`<!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Welcome to CodeIgniter</title>
      <link rel="stylesheet" href="<?php echo base_url(); ?>css/bootstrap.css">
      <script src="<?php echo base_url(); ?>js/jquery.js"></script>
      <script src="<?php echo base_url(); ?>js/bootstrap.min.js"></script>
    </head>
    <body>
    <div class="container">
      <div class="row">
        <div class="col-sm-4">
          <h2 class="page_header">Selamat datang di CodeIgniter + Boostrap</h2>
          <form>
            <div class="form-group">
              <label>Nama</label><br>
              <input type="text" class="form-control" placeholder="Nama Lengkap">
              <label>Alamat</label><br>
              <textarea type="text" class="form-control" cols="40" rows="5" placeholder="Alamat"></textarea>
              <label>Tempat Lahir</label><br>
              <input type="text" class="form-control" placeholder="Tempat Lahir">
              <label>Tanggal Lahir</label><br>
              <input type="date" class="form-control" placeholder="Tanggal Lahir"><br>
              <button class="btn btn-danger" type="submit">Simpan</button>
            </div>
          </form>
        </div>
      </div>
    </div>
    </body>
    </html>`
