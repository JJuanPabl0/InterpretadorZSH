# Instalação do Zsh no Ubuntu  

## O que é o Zsh?  
O **Zsh (Z Shell)** é um shell de linha de comando avançado que oferece mais recursos do que o Bash, incluindo:  
- **Autocompletar inteligente** (com sugestões baseadas no histórico)  
- **Navegação aprimorada entre diretórios**  
- **Suporte a plugins e temas** (como o Oh My Zsh)  
- **Melhoria no histórico de comandos**  
- **Sugestões automáticas de correção de comandos digitados errados**  

---

## Como instalar o Zsh no Ubuntu  

### 1. Atualizar os repositórios do sistema  
```bash
sudo apt update && sudo apt upgrade -y
```

### 2. Instalar o Zsh
```bash
sudo apt install zsh -y
```
### 3. Verificar se a instalação foi bem-sucedida
```bash
zsh --version
```
Se aparecer algo como zsh 5.x.x, a instalação foi concluída com sucesso.

### 4. Definir o Zsh como shell padrão
```bash
chsh -s $(which zsh)
```
Isso fará com que o Zsh seja o shell padrão em vez do Bash.


### 5. Reiniciar o terminal
Feche e abra o terminal novamente para que o Zsh seja carregado como padrão.

## **(Opcional) Instalar o Oh My Zsh**
O Oh My Zsh é um framework que adiciona temas e plugins ao Zsh, tornando-o mais personalizável.

### 1. Instalar dependências necessárias
```bash
sudo apt install curl git -y
````

### 2. Baixar e instalar o Oh My Zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### 3. Editar o arquivo de configuração do Zsh
Após a instalação, edite o arquivo de configuração para personalizar temas e plugins:
```bash
nano ~/.zshrc
```

### 4. Recarregar o Zsh para aplicar mudanças
```bash
source ~/.zshrc
```

Agora seu terminal está com o Zsh funcionando e, se desejar, com o Oh My Zsh para melhorar a experiência! 🚀
