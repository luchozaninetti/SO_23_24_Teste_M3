# Teste de Sistemas Operativos - Módulo 3

Faz *fork* do repositório para teres a tua cópia.

Preenche o ficheiro README diretamente no GitHub. A partir da página principal do repositório, clica em "Edit File" (ícone representando um lápis).

Escreve as respostas dentro dos blocos correspondentes. Substitui as reticências pelo que é pedido em cada pergunta. Não desformates o documento.

Quando acabares, carrega no botão "Commit Changes".

## Informação do aluno

    Nome: Luis Fernando Zaninetti 11Q1

## P1 - Para as seguintes questões, assinala a opção correta: (2.5v)

  1. Qual das seguintes afirmações caracteriza melhor um SO servidor?

    a) Projetado para computação de uso geral
    b) Otimizado para alta disponibilidade e confiabilidade
    c) Destinado a usuários individuais
    d) Usado principalmente para jogos
    
    Resposta: A

  2. Das seguintes, qual é a função mais apropriada para um SO servidor?

    a) Executar aplicações de desktop
    b) Desenvolver aplicações móveis
    c) Fornecer software de entretenimento
    d) Gerir recursos e serviços de rede
    
    Resposta: D
   
  3. Qual dos seguintes é um sistema operativo servidor popular?

    a) Windows 11
    b) macOS Big Sur
    c) Ubuntu Server
    d) Android
    
    Resposta: C

  4. Qual é o papel de um servidor num modelo cliente-servidor?

    a) Consumir recursos fornecidos pelos clientes
    b) Fornecer recursos e serviços aos clientes
    c) Atuar como uma estação de trabalho independente
    d) Facilitar a comunicação ponto a ponto
    
    Resposta: B

  5. Qual dos seguintes protocolos é mais usado para aceder remotamente a servidores?

    a) FTP
    b) HTTP
    c) SSH
    d) SMTP
    
    Resposta: B

## P2 - Indica, sequencialmnente, os comandos para realizar as seguintes instruções: (7.5v)

  1. Cria um diretório com o nome "ex1", entra no mesmo, e cria 3 ficheiros vazios com os nomes "f1", "f2", "f3". No fim, lista os conteúdos do diretório atual.

    Resposta:
    mkdir ex1
    cd ex1
    touch f1
    touch f2
    touch f3
    ls
    
  2. Assumindo que estás no diretório "ex1", renomeia os ficheiros "f1" e "f2" para que acabem com "_antigo", e cria cópias dos mesmos.

    Resposta:
    mv f1 f1_antigo
    mv f2 f2_antigo
    cp -r f1_antigo f4
    cp -r f2_antigo f5
    
  3. Assumindo que estás no diretório "ex1", cria o diretório "ex2", e move os ficheiros copiados no exercício anterior para o novo diretório. Seguidamente, apaga os ficheiros originais.

    Resposta:
    sudo mv f4 ex2
    sudo mv f5 ex2
    rm f1_antigo
    rm_f2antigo

  4. Atualiza os repositórios de *packages* para garantir acesso às *packages* mais recentes, e instala o serviço **htop**.

    Resposta:
    sudo apt uptade
    sudo apt install htop

  5. Cria um novo utilizador com o teu primeiro nome, e com o diretório "/home/nome_de_utilizador". Mostra a informação (ID) do utilizador criado.

    Resposta:
    sudo adduser luis
    mkdir luis
    su luis
    id

## P3 - Realiza os seguintes exercícios, com respostas detalhadas: (6v)

  1. Indica alguns aspetos que diferenciam um SO cliente de um SO servidor.

    Resposta: 
    O cliente inicia pedidos para servidores, espera por respostas e recebe respostas, já o servidor recebe os pedido e manda as informações que o cliente solicita
            
    
     
  2. Explica a importância de otimizar um sistema operativo servidor, com exemplos de técnicas para otimização.

    Resposta: Atualizações trazem melhorias e novidades e também corrigem possíveis problemas e falhas.
    

  3. Descreve o processo de instalar e configurar um servidor web num SO servidor, incluindo as etapas necessárias.

    Resposta:
    1º atualizamos os repositorios; 2º Instalação do Apache; 3º iniciar o Apache; 4º Habilitar no Boot, para garantir que o Apache seja iniciado automaticamente durante o boot do sistema.

## P4 - Indica os comandos **git** para realizar as seguintes operações: (4v)

  1. Considera que estás no ramo 'master' de um repositório git criado localmente. Associa este repositório ao repositório remoto contido no url 'https://github.com/SO/OMeuRepositorioRemoto'. Altera o nome do ramo atual para 'main', e envia os *commits* já feitos localmente para o repositório remoto.

    Resposta: git remote add origin https://github.com/SO/OMeuRepositorioRemoto
            git branch -m master main
            git push -u origin main
            

  2. Considera que estás na pasta raiz do teu repositório local, onde atualizaste um ficheiro de nome 'index.html'. Envia **apenas** esta atualização para o teu repositório remoto, com uma mensagem de commit apropriada.

    Resposta:
    git add index.html
    git commit -m "Atualização do arquivo index.html"
    git remote add origin (url_do_repositori)


