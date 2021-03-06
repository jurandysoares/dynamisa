# Diário
Crie uma estrutura de diretórios para um diário de atividades do ano.

## Objetivos
* Avaliar suas habilidades de criação de diretórios (`mkdir`)
* Avaliar suas habilidades de exclusão de diretórios (`rmdir` ou `rm -rf`)
* Avaliar suas habilidades de navegação em diretórios (`cd` e `pwd`)
* Avaliar suas habilidades de listagem de arquivos (`ls`)
* Avaliar suas habilidades de criação de arquivos por meio de redirecionamento de saída (`>` ou `>>`)
* Avaliar suas habilidades de exibição de conteúdo de arquivos (`cat`, `less`, `view`, `nano`)
* Exibir variáveis de ambiente (`env`, `set`, `set | less`)
* Alterar variáveis de ambiente (`VAR=valor`. Ex.: `PS1='[\W]$ '`)
* Concatenar arquivos (`cat arq1.txt arq2.txt arq3.txt > arq4.txt`)
* Copiar arquivos e pastas (`cp`, `cp -r`, `cp -v`, `cp -i`, `cp -f`)
* Excluir arquivos e pastas (`rm` e `rm -r`)

## Dicas para navegação em diretório
|Símbolo|Descrição|Exemplo|
|:---:|:---|---|
|.|Diretório atual (`pwd`)|`./comando`|
|..|Diretório pai (superior)|`ls ../`; `ls ../../`; `cd ..`|
|~|Diretório HOME (pasta base do usuário) |`cd ~/Documents`|
|-|Diretório anterior|`cd -`|

## Instruções
Para criação dos arquivos \<index.md>, você deverá utilizar *[here document](https://es.wikipedia.org/wiki/Here_document)*:
```bash
cat << FIM > index.md
[...]
FIM
```

## Roteiro

### Pasta de modelo para um dia
1. Crie uma pasta chamada `dia` e dentro dela crie as subpastas:
* `manha`
* `tarde`
* `noite`

2. Dentro da pasta `dia`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Dia
* [Manhã](./manha/)
* [Tarde](./tarde/)
* [Noite](./noite/)
* [Mês](../)
```

3. Dentro da pasta `manha`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Manhã
* [Dia](../)
```

4. Dentro da pasta `tarde`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Tarde
* [Dia](../)
```

5. Dentro da pasta `noite`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Noite
* [Dia](../)
```

### Estrutura de um diário
1. Crie a pasta `diario` e dentro dela crie as subpastas:
* `jan`
* `fev`
* `mar`
* `abr`
* `mai`
* `jun`
* `jul`
* `ago`
* `set`
* `out`
* `nov`
* `dez`

2. Dentro da pasta `diario`, crie o arquivo `index.md` com o seguinte conteúdo:
```
# Diário de ${USER}
* [Janeiro](./jan/)
* [Fevereiro](./fev/)
* [Março](./mar/)
* [Abril](./abr/)
* [Maio](./mai/)
* [Junho](./jun/)
* [Julho](./jul/)
* [Agosto](./ago/)
* [Setembro](./set/)
* [Outubro](./out/)
* [Novembro](./nov/)
* [Dezembro](./dez/)
* [Calendário](../)
```
### Primeiro dia do diário
1. Entre na pasta do mês atual (Ex.: `cd jul`)
2. Copie a pasta `dia` com o número dia de hoje (Ex.: `cp -rv ../dia 28`)
3. Faça isso para todos os dias do mês

Se você gosta de programação, exprimente resolver o problema anterior com programação em Shell Script.
```bash
# Aquecimento
# *do* ("faça" em Inglês) corresponde ao abre chaves ({) do C/Java
# *done* ("feito" em Inglês) corresponde ao fecha chaves (}) do C/Java
###
# Exemplo 1: *For* clássico
for ((d=1; d<=31; d++))
  do
    echo $d
  done

###
# Exemplo 2: *For* mais simples
for d in {1..31}
  do
    echo $d
  done

###
# Exemplo 3: *For* que faz a cópia da pasta *dia* para cada dia do mês de julho
for d in {1..31}
  do
    echo "Criação da pasta para o dia ${d}..."
    cp -rv ~/dia $d
  done
```
