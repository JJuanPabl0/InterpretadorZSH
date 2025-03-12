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


