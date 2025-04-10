# Anotações da aula
A aula sobre git foi essencial para compreender os principais comandos e funcionalidades do git.

## Conceitos abordados na aula
- Servidores geralmente não possuem interface gráfica (GUI), apenas linha de comando (CLI).
- Discussão sobre segurança do Linux x Windows;
- Introdução ao processo de Deploy com DevOps;
- Diferença entre repositório local e remoto;
- O que é o HEAD e como ele se movimenta;
- Como surgem e como resolver conflitos;
- Criação e gerenciamento de branchs;
- Como realizar merges com segurança.

## Comandos explorados
<b>Navegação e diretórios</b> </br>
```
pwd                                  # Mostra o caminho do diretório atual
mkdir nome_pasta                     # Cria uma nova pasta
cd ..                                # Volta um diretório
cd /                                 # Vai para o diretório raiz
cd ~                                 # Vai para o diretório pessoal
cd ~/aula_terminal                   # Acessa pasta específica
```

<b>Criação de arquivos e diretórios</b>
```
mkdir outono inverno primavera                    # Cria várias pastas
touch java.txt sql.txt javascript.txt cobol.txt   # Cria arquivos
```

<b>Listagem de arquivos</b>
```
ls -l                      # Mostra detalhes dos arquivos (permissões, dono, data etc.)
ls -ld                     # Mostra detalhes da pasta atual
ls -a                      # Mostra também arquivos ocultos
```

<b>Manipulação de Arquivos</b>
```
cat cobol.txt                      # Exibe o conteúdo
nano cobol.txt                     # Edita com o editor nano
cp cobol.txt ./inverno             # Copia arquivo para pasta
cp sql.txt sql2.txt                # Cria cópia com novo nome
cp cobol.txt java.txt ./verao      # Copia vários arquivos
cp -r ./verao/ ./outono/           # Copia pasta e subpastas
mv sql.txt ./primavera             # Move arquivo
mv sql2.txt slq.txt                # Renomeia arquivo
rm javascript.txt                  # Remove arquivo
rmdir ./outono                     # Remove pasta (se estiver vazia)
rm -r nome_pasta                   # Remove pasta e conteúdo, permite a remoção recursiva
rm -rf nome_pasta                  # Remove sem pedir confirmação, força a exclusão
```

<b>Comandos de reset e restauração</b>
```
git reset                              # Volta alterações sem apagar
git reset --hard                       # Volta e apaga alterações
git restore arquivo                    # Restaura arquivo do último commit
git restore --staged                   # Remove arquivo da staging area
```

## Configurações Git úteis
```
git config --global core.editor "code --wait"      # Define VS Code como editor padrão
git config --global pull.rebase false              # Desativa rebase no pull
```