unopar-lamp
===========

Servidor LAMP (Linux, Apache, MySQL, PHP) para desenvolvimento de aplicações Web - Unopar

Configuração do Vagrant (com script de provisionamento) para criar uma máquina virtual (Ubuntu 12.04) de desenvolvimento em PHP, para atividades da disciplina de Desenvolvimento Web.

Também é instalado o PHPMyAdmin para gerenciamento do MySQL.

A senha padrão para todos os serviços é *unopar*.

Pré-requisitos
==============

Git - http://git-scm.com/
Vagrant - http://www.vagrantup.com/
Virtualbox - https://www.virtualbox.org/
Conexão com a Internet

Aviso
=====

Esse documento trata apenas ao uso dessa máquina virtual. O uso do git, vagrant e virtualbox está fora do escopo desse documento. Porém existem diversos tutoriais sobre essas ferramentas na Internet. O conhecimento sobre elas não é obrigatório para o uso dessa máquina virtual, mas é recomendado.

Modo de Uso
===========

* Clone esse repositório para sua máquina:

- git clone https://github.com/psychopenguin/unopar-lamp-vagrant.git

* Entre no diretório unopar-lamp-vagrant

* Inicie a máquina com o vagrant

- vagrant up

Após algum tempo, variavel de acordo com a velocidade de sua conexão, sua máquina virtual estará pronta.

A primeira vez será um pouco mais demorada, pois o vagrant precisa baixar a imagem da máquina virtual.

Quando a máquina virtual estiver pronta, um servidor web estará disponível no endereço http://localhost:8080, e a instalação do PHPMyAdmin está em http://localhost:8080/phpmyadmin.

Coloque seu código no diretório *www-data*. Todo o conteúdo dele estará disponível para uso no apache.

O mesmo já tem um arquivo index.php que chama a função phpinfo().
Para desligar a máquina virtual utilize o comando:

- vagrant halt

Para religar novamente utilize:

- vagrant up

Caso queira destruir a máquina virtual (o conteúdo do www-data não será perdido):

- vagrant destroy

Abraços!
