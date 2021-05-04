# Webhooks
Webhooks disparados quando algumas ações são feitas no sistema.



**Observação: Informe a SOHTEC o EndPoint que irá receber os POSTs do sistema.**



**Modelos de JSONs enviados para cada ação feita no sistema.**

Com a **chave(key)** do cliente fornecida pela SOHTEC siga os passos abaixo.

**Proposta enviada**
```javascript {.line-numbers}
{
   "nome":"Fulano",
   "email":"fulano@email.com.br",
   "telefone":"",
   "codigoImovel":"0002",
   "propostaAceita":true,
   "valorAtual":"1.250,00",
   "valorNovo":"22,00",
   "tipoWebhook":"PROPOSTA"
}
```

**Visita confirmada**
```javascript {.line-numbers}
{
   "email":"fulano@email.com.br",
   "nome":"Fulano",
   "telefone":"000000000",
   "cpf":"000.000.000-00",  
   "imovelId":"0002",
   "dataAgendamento":"06/05/2021 09:00",
   "modulo":"LOCACAO",
   "tipoWebhook":"AGENDAMENTO_VISITA"
}
```

**Novo Lead**
```javascript {.line-numbers}
{
   "nome":"Fulano",
   "email":"fulano@email.com.br",
   "telefone":"51995486882",
   "codigoImovel":"0002"
}
```

