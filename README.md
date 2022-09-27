# Disparo de E-mails com Anexo

O arquivo `Gerentes.xlsx` contém uma lista com os contatos dos gerentes de uma empresa fictícia para os quais desejamos enviar e-mails personalizados, anexando planilhas com os dados de suas respectivas áreas.

A empresa possui as seguintes áreas:

- Financeiro
- Logística
- Manutenção
- Marketing
- Operações
- Produção
- Vendas

O template dos e-mails que pretendemos enviar tem a seguinte forma:

```python
texto = f'''
Prezado, {nome_gerente},
Segue em anexo o Relatório de {area}.
Att.,
Diego Moura Torres
'''
```

Usando o módulo `yagmail`, foi possível enviar os e-mails para cada um dos gerentes.

## Observação

Os dados de autenticação foram guardados em um arquivo `.env`, o qual não está presente neste repositório.

Caso queira reproduzir a solução apresentada neste notebook, crie um arquivo `.env` com a seguinte estrutura:

```txt
NOME_USUARIO=meuemail@gmail.com
SENHA=minhasenha
```
