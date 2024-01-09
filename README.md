# Instruções para instalação do Zsh e Oh-my-zsh.
***

## **Zsh:**
- Para instalar o zsh digite a linha de comando abaixo no terminal do Linux:</br>
`sudo apt install zsh` </br></br>
- Após a instalação, para configurar o Zsh como bash padrão, edit com o NANO o arquivo _**/etc/passwd**_ conforme comando a seguir:</br>
`sudo nano /etc/passwd`

Procure pela linha onde consta o nome do seu usuário, ela deve estar mais no final do arquivo, logo ao final da linha **”/bin/bash“**, tudo o que temos a fazer aqui é trocar a palavra **“bash”** por **“zsh“**. Veja na tela abaixo onde na linha em destaque aparece o nome do usuário e a referência a **"bin/bash"**. No local de **"bash"** coloque **"zsh"** salve o arquivo e reinicie o sistema para o Zsh se tornar o bash padrão.</br></br>

<img src="/Images/arq_etc_pws.png">

## **Oh-my-zsh:**
<img src="/Images/ohmyzsh.png">

- **Instalação do git, curl e winget:** Antes da instalação do **Oh-my-zsh** instale as ferramentas **git, curl e winget** digitando o seguinte comando no terminal do Linux: </br>
`sudo apt install git curl winget`

- **Instalação do Oh-my-zsh:** Para instalação do **Oh-my-zsh** digite o seguinte comando no terminal do Linux: </br>
  `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- **Instalação da fonte Firacode:** Instale a fonte **Firacode** utilizando o seguinte comando no terminal do Linux: </br>
  `sudo apt install fonts-firacode`
    - A fonte Firacode é uma fonte que proporciona um visual mais agradável do texto e do prompt do terminal quando começamos a utilizar o Oh-my-zsh, pois algumas fontes podem gerar caracteres e símbolos que não agradam ao usuário. Após a instalação da fonte firecode reinicie o terminal.
- **Alteração da fonte do terminal:** Abra o terminal para alterar a sua fonte. Para isso clique em **Editar -> Preferências -> Aparência** e no campo *fonte* selecione **Fira Code Light** e escolha o tamanho da fonte que desejar em seguida feche a janela de configuração e reinicie o terminal para que a alteração da fonte surta efeito.
- **Alteração do tema do Oh-my-zsh:** para alterar o tema do Oh-my-zsh edite com o **NANO** o arquivo **.zshrc** e na linha onde constar **ZHS_THEME="robbyrussel"** alterar o tema para **"agnoster"** que proporcionará um visual agradável no prompt do terminal. Após a alteração no tema, salve o arquivo com **CTRL+O** e saia do **NANO** com **CTRL+X**. Para edição do arquivo use o comando a seguir:</br>
`sudo nano ~/.zshrc`
  - Para que a alteração do tema surta efeito feche o terminal e abra novamente ou então digite o seguinte comando no terminal:
  <br>`source ~/.zshrc`
### **Instalação dos plugins do Oh-my-zsh:**
- **Zsh-Syntax-highlighting:** esse plugin é utilizado para iluminar, ou seja, para destacar os comandos enquanto eles são digitados. Dessa forma, se o comando estiver correto, ele será exibido na cor verde, caso contrário, o comando ficará em vermelho. Isso facilita o trabalho da pessoa programadora, pois ela poderá identificar com facilidade quando digitar um comando errado. Para instalação do plugin digite o seguinte comando no terminal:</br>
  `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

- **Zsh-autosuggestions:** esse plugin é extremamente útil para as pessoas desenvolvedoras, pois ele faz a sugestão de comandos com base no que já foi digitado. Portanto, ele funciona como uma ferramenta para autocompletar o que está sendo digitado. Para instalação do plugin digite o seguinte comando no terminal:</br>
`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

- **Fzf:** esse plugin possibilita a pesquisa de arquivos e pastas pelo terminal de forma simples e rápida, além de comandos já digitados. Para baixar e instalar o plugin digite os seguintes comandos no terminal:</br>
```
git clone --depth 1 https://github.com/junegunn/fzf.git~/.fzf
~/.fzf/install
```
- **K:** é útil para exibir detalhes como a data de criação, o tamanho e as permissões de uso de arquivos e pastas. Para instalar essa ferramenta, basta digitar o seguinte comando em seu terminal: </br>
`git clone https://github.com/supercrabtree/k $ZSH_CUSTOM/plugins/k`

- **Adicionar os plugins no arquivo .zshrc:** O próximo passo é adicionar os nomes dos plugins na relação de plugins instalados, Portanto, veja como ficará a configuração dos plugins no arquivo **.zshrc** o qual deverá ser editado com o **NANO**:
  - Edite o arquivo **.zshrc** conforme o comando a seguir:</br>
 `sudo nano ~/.zshrc`
  - Na linha do arquivo onde se encontra as sessões de plugins você verá que já existe o plugin *git*, digite após ele os nomes dos demais puglins separados por espaço, salve o arquivo com **CTRL+O** e saia do **NANO** com **CTRL+X**. A linha onde conterá os plugins deverá ficar semelhante a imagem abaixo:</br>
<img src="/Images/plugins.png">

  - Além dos plugins que foram instalados, consta na imagem acima os seguintes plugins os quais já integram o oh-my-zshell, bastando incluí-los na lista de plugins no arquivo **.zshrc**, a saber:</br>
    -  **colored-man-pages:** Este plugin adiciona cores às páginas do comando *man* (manual)
    -  **web-search:** Este puglin permite consultas no google que podem ser acionadas a partir do terminal do Linux digitando-se por exemplo **"google plugins"** o que fará com que o navegador abra uma pagina com links para pesquisar o termo ou palavra desejado, que neste caso foi indicada a palavara *plugins*.
    -  **dircycle:** Este plug-in permite a você alternar/navegar entre pastas/diretórios acessados no terminal do Linux. Ele usa um pequeno truque que permite percorrer os diretórios acessados para a esquerda ou para a direita usando Ctrl+ Shift+ Left/ Right.

[Clique no link abaixo para acessar o site onde constam boas dicas para instalação do Zsh e Oh-my-zsh] (https://blog.betrybe.com/ferramentas/oh-my-zsh/)








