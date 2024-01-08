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
    - A fonte Firecode é uma fonte que proporciona um visual mais agradável do prompt quando começamos a utilizar o Oh-my-Zshell, pois algumas fontes podem gerar caracteres e símbolos que não agradam ao usuário. Após a instalação da fonte firecode reinicie o terminal.







