# Instruções para instalação do Zsh e Oh-my-zshell.
***

## **Zsh:**
- Para instalar o zsh digite a linha de comando abaixo no terminal do Linux:</br>
`sudo apt install zsh` </br></br>
- Após a instalação, para configurar o Zsh como bash padrão, edit com o NANO o arquivo _**/etc/passwd**_ conforme comando a seguir:</br>
`sudo nano /etc/passwd`

Procure pela linha onde consta o nome do seu usuário, ela deve estar mais no final do arquivo, logo ao final da linha **”/bin/bash“**, tudo o que temos a fazer aqui é trocar a palavra **“bash”** por **“zsh“**. Veja na tela abaixo onde na linha em destaque aparece o nome do usuário e a referência a **"bin/bash"**. No local de **"bash"** coloque **"zsh"** salve o arquivo e reinicie o sistema para o Zsh se tornar o bash padrão.</br></br>

<img src="/Images/arq_etc_pws.png">

## **Oh-my-zshell:**
<img src="/Images/ohmyzsh.png">

- Antes da instalação do **Oh-my-zshell** instale as ferramentas **git, curl e winget** digitando o seguinte comando no terminal do Linux: </br>
`sudo apt install git curl winget`

- Em seguida para instalação do **Oh-my-zshell** digite o seguinte comando no terminal do Linux: </br>
  `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- Instale a fonte **Firacode** utilizando o seguinte comando no terminal do Linux: </br>
  `sudo apt install fonts-firacode`
    - A fonte Firacode é uma fonte que proporciona um visual mais agradável do texto e do prompt do terminal quando começamos a utilizar o Oh-my-Zshell, pois algumas fontes podem gerar caracteres e símbolos que não agradam ao usuário. Após a instalação da fonte firecode reinicie o terminal.
- Abra o terminal para alterar a sua fonte. Para isso clique em **Editar -> Preferências -> Aparência** e no campo *fonte* selecione **Fira Code Light** e escolha o tamanho da fonte que desejar em seguida feche a janela de configuração e reinicie o terminal para que a alteração da fonte surja efeito.
- **Alteração do tema do Oh-my-Zshell:** para alterar o tema do Oh-My-Zshell edite com o **NANO** o arquivo **.zshrc** e na linha onde constar **ZHS_THEME="robbyrussel"** alterar o tema para **"agnoster"** que proporcionará um visual agradável no prompt do terminal. Após a alteração no tema, salve o arquivo com *CTRL+O* e saia do **NANO** com *CTRL+X*. Para edição do arquivo use o comando a seguir:</br> `
`sudo nano zshrc`





