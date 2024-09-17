## SERVIDORES EMAIL e WEBMAIL - DOVECOT E POSTFIX  :bookmark_tabs:

Nessa pasta foi criado um dockerfile para criação de servidores de email **Postfix** como **SMTP**, **Dovecot** como **IMAP** e **WEBMAIL**. Com algumas alterações no **main.cf** nas configurações do postfix, **10-mail.conf**, **10-master.conf**, **20-pop3.conf** e **dovecot.conf** nas configurações do dovecot.


## WEBMAIL - RAINLOOP
Foi criado um dockerfile para criação de um webmail através de uma imagem **debian** configurado a um apache, configurado a serviços de proxy e de DNS apontando para o dominio **asa.br**


Para acessar o WEBMAIL é só acessar usando **www.asa.br:8080/rainloop/**, assim você cairá na pasta padrão de login para usuário comum entrar, já se acessar com **www.asa.br:8080/rainloop/?admin#/domains**, estará acessando como administrador, para efetuar as configurações. O usuário é *admin* e a senha é *12345*.
