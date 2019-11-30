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
