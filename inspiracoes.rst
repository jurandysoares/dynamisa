Inspirações
=============

* Abecedário: Estava eu passando em frente ao Frasqueirão, estádio do time do ABC de Natal. Gabarito em Python para criação da árvore de diretório de uma turma específica de 2016::

   import os,grp,pwd
   
   so2016 = grp.getgrnam('so2016').gr_mem
   
   for u in so2016:
       detox_name = pwd.getpwnam(u).pw_gecos.split(',')[0].split(' ')[0].replace(' ','_')
       os.makedirs('/tmp/abecedario/{}'.format('/'.join(list(detox_name))))

* UAU: Página 20 do livro `«A natureza ensina» <http://www.travessa.com.br/a-natureza-ensina/artigo/da4f3a53-62f7-4bd4-b0ac-44a633d654b0>`_, de Peter Miller. Mecanismos de auto-organização da natureza:

  * Controle descentralizado
  * Resolução de problemas de forma distribuída
  * Interações múltiplas
