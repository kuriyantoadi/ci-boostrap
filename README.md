# CodeIgniter-Boostrap
Menghubungkan CI dan Boostrap

1. Extrak Framework CI dan Boostrap

2. application/config/config.php baris 26
  Awal :
    $config['base_url'] = '';
  Edit :
    $config['base_url'] = 'http://localhost/ci-boostrap';

3. application/config/autoload.php baris 92
  Awal :
    $autoload['helper'] = array('');
  Edit :
    $autoload['helper'] = array('url');
