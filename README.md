# Criando Ambiente de Desenvolvido COBOL no Windows e Utlizando o VSCode

1. Baixar o VSCode - buscar no Google;

2. Instalar o VSCode (seguir as instruçoes);

3. Após instalar, abrir o VSCode e instalar a extensao "IntelliSense - Highlight" apenas;

4. Baixar os binários do GNU COBOL para Windows (compilados) 
   em: https://drive.google.com/file/d/1vxzD... (link na descricao do video)

5. Criar uma pasta na unidade raiz (geralmente, c:\) - Exemplo: C:\GNUCOBOL;

6. Fazer as configuraçoes das variaveis de ambiente em "Variaveis do Sistema":<br>
   6.1. Criar a variavel COBOL_HOME e apontar para o diretorio principal do GNU COBOL;<br>
   6.2. Criar as variaveis:<br>
        &nbsp6.2.1. COB_BIN_DIR:  apontar para sub-diretorio "bin" do GNU COBOL;<br>
        &nbsp6.2.2. COB_CONFIG_DIR : apontar para sub-diretorio "config" do GNU COBOL;<br>
        &nbsp6.2.3. COB_COPY_DIR: apontar para sub-diretorio "copy" do GNU COBOL;<br>
        &nbsp6.2.4. COB_INCLUDE_PATH: apontar para sub-diretorio "lib" do GNU COBOL;

7. Adicionar as variaveis de ambiente de sistema na variável "path" do sistema<br>
    7.1. COBOL_HOME: Para criar no Path %COBOL_HOME%;<br>
    7.2. COB_BIN_DIR: Para criar no Path %COB_BIN_DIR%;<br>
    7.3. COB_CONFIG_DIR: Para criar no Path %COB_CONFIG_DIR%;<br>
    7.4. COB_COPY_DIR: Para criar no Path %COB_COPY_DIR%;<br>
    7.5. COB_INCLUDE_PATH: Para criar no Path %COB_INCLUDE_PATH%;<br>

8. Abrir um prompt de comando e testar a chamada com "cobc -v";

9. Se der tudo certo, criar uma workspace e um diretório no VS Code e criar um 
   arquivo testecob.cob nele;

10. Digitar um código COBOL básico (só pra testar);
    
11. Abrir um novo terminal no VS Code, acessar o diretório e compilar o código criado.<br>
    11.1. Para executar o código no terminal na pasta raiz onde está localizado o código
          execute o comando de compilação: cobc -x testecob.cob<br>
    12.2. Para visualizar o exe gerado no terminal na pasta onde gerou o exe execute o comando: 
          testecob.exe
