

# Docker RUNDECK


refs.:

https://github.com/rundeck/rundeck

https://computingforgeeks.com/install-and-configure-rundeck-on-ubuntu-18-04-lts/

Instalar Rundeck e rodar

1) cria um diretorio na ./ #mkdir rundeck3
2) cd rundeck3
3) git clone https://github.com/mlucasdasilva/rundeck

ira fazer clone dos arquivo e criará um diretorio rundeck

4) entrar no diretorio #cd rundeck
5) #ls -l
6) #vi docker-compose.yml
7) em hostname colocar o ip de acesso ao rundeck
   #192.168.56.105.nip.io
8) #docker-compose build
9) #docker-compose up -d (subir docker e rundeck)

10) #docker-compose logs -f (Ver Logs e verificar se subiu a aplicação)
11) após ir ao navegador e digitar o ip configurado no docker-compose.yml no meu caso http://192.168.56.105.nip.io:4440

12) irá aparecer a pagina do Rundeck, log com o login: admin senha: admin

13 para deruubar o docker e o rundeck rode o comando # docker-compose down 

Grupo Trabalho Rundeck (Diciplina Tópicos especiais)


Wagner Simões

Thiago Passos

Waldir Bravin

Andre  Gomes



Professor Marcelo Lucas

Senac RJ (Centro Tecnológico)

Rede de Computadores.

_____________________________

gradecemos a todos os que nos apoiaram!

#rundeck

