# Calendário
1. Crie uma pasta chamada `cal` e dentro dela crie as pastas:
* `dia`
* `semana`
* `ano`

2. Dentro da pasta `cal`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Calendário
* [Dia](./dia/)
* [Semana](./semana/)
* [Ano](./ano/)
```
Para criação do arquivo, você só poderá utilizar o comando `echo` e redirecionamento de saída padrão com `>` ou `>>`.

Converta o arquivo `index.md` para o formato HTML. Dica: Use a ferramenta [Pandoc](http://pandoc.org/).

3. Dentro da pasta `dia`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Dia
* [Calendário](../)
```

Converta o arquivo `index.md` para o formato HTML. Dica: Use a ferramenta [Pandoc](http://pandoc.org/).

4. Dentro da pasta `semana`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Semana
* [Calendário](../)
```

Converta o arquivo `index.md` para o formato HTML. Dica: Use a ferramenta [Pandoc](http://pandoc.org/).

5. Dentro da pasta `ano`, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Ano
* [Calendário](../)
```

Converta o arquivo `index.md` para o formato HTML. Dica: Use a ferramenta [Pandoc](http://pandoc.org/).

Terminadas as atividades acima, sigas as intruções para:
* [Dia](#dia) 
* [Semana](#semana)
* [Ano](#ano)

<a name="dia">

## Subpastas de um Dia
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
* [Calendário](../)
```

Converta o arquivo `index.md` para o formato HTML. Dica: Use a ferramenta [Pandoc](http://pandoc.org/).

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

5. Dentro da pasta ``, crie o arquivo chamado `index.md` com o seguinte conteúdo:
```
# Noite
* [Dia](../)
```

<a name="semana">

## Subpastas de uma Semana
Crie uma pasta chamada `semana` e dentro dela crie as subpastas:
* `seg`
* `ter`
* `qua`
* `qui`
* `sex`
* `sab`
* `dom`



<a name="ano">

## Subpastas de um Ano
Crie uma pasta chamada `ano` e dentro dela crie as subpastas:
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
