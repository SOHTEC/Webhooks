# Webhooks
Webhooks disparados quando algumas ações são feitas no sistema.

**Observação:** Informe a SOHTEC o EndPoint que irá receber os POSTs do sistema.

**Modelos de JSONs enviados para cada ação feita no sistema.**

**Proposta enviada**
```javascript {.line-numbers}
{
    "garantia": "",
    "nome": "",
    "email": "",
    "telefone": "",
    "proprietarios": [
        {
            "nome": "",
            "email": "",
            "telefone": ""
        }
    ],
    "codigoImovel": "",
    "valorAtual": "",
    "valorNovo": "",
    "tipoWebhook": "PROPOSTA",
    "quemFezAcao": "",
    "corretorCodigo": "",
    "acao": ""
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
   "nome":"",
   "email":"",
   "telefone":"",
   "codigoImovel":"",
   "imovel":{
        "endereco":"",
        "numero":"",
        "complemento":"",
        "cidade":"",
        "estado":"",
        "cep":"",
        "foto":"",
        "dormitorios":"",
        "garagem":"",
        "valor":"",
        "iptu":"",
        "condominio":"",
        "proprietarios":[],       
   },
   "corretorCodigo":"",
   "interesse":"", 
   "origem":"",
   "tipoWebhook":"WEBHOOK_LEADS"
}
```

