---
# **Apresentação sobre Comandos e Conceitos do Linux**

## **1. Como listar todos os arquivos em um diretório no Linux usando o terminal?**

- Use o comando `ls` no terminal.
- Para listar arquivos em um diretório específico:
  ```bash
  ls /caminho/do/diretorio


Para listar arquivos detalhadamente com permissões, tamanho e data de modificação:


```
ls -l
```

Para incluir arquivos ocultos:

```
ls -a
```

Para listar arquivos em ordem recursiva (incluindo subdiretórios):


```
ls -R
```

## **2. O que é o sudo no Linux e por que é frequentemente usado em comandos administrativos?**

Sudo significa "Super User Do".
Permite a execução de comandos com permissões de superusuário ou administrador.
É frequentemente usado porque:
Garante a segurança ao permitir que usuários executem comandos elevados sem logar como root.
Restringe o uso de privilégios elevados apenas a comandos específicos.
Exemplo:
bash

```
sudo apt update
```


Neste exemplo, o comando apt update é executado com permissões administrativas.


## **3.Qual é a diferença entre os diretórios /etc, /bin e /home no sistema de arquivos Linux?**

Diretório	Descrição
/etc	Contém arquivos de configuração do sistema e aplicativos. Exemplos: /etc/hosts, /etc/passwd.
/bin	Contém binários essenciais usados pelos usuários e pelo sistema. Exemplos: ls, cat, cp.
/home	Diretório pessoal dos usuários. Cada usuário possui uma pasta separada. Exemplo: /home/usuario.


## **4.Como procurar um texto específico dentro de arquivos em um diretório e seus subdiretórios no Linux?**

Utilize o comando grep com a opção -r para busca recursiva.

Sintaxe:


```
grep -r "texto_procurado" /caminho/do/diretorio

```

Para ignorar diferenciação entre maiúsculas e minúsculas, adicione a opção -i:


```
grep -ri "texto_procurado" /caminho/do/diretorio

```

Para mostrar apenas os nomes dos arquivos que contêm o texto:


```
grep -rl "texto_procurado" /caminho/do/diretorio

```

Exemplo prático:

```
grep -r "error" /var/log/
```

