# PDF Vencimento API

API Node.js para extrair a primeira data (dd/mm/yyyy) de arquivos PDF enviados via `multipart/form-data`.

## Endpoint

`POST /extrair-vencimento`

### Body

- Form-data com campo `pdf` (arquivo binário)

### Retorno

```json
{
  "vencimento_br": "15/01/2025",
  "vencimento_iso": "2025-01-15T00:00:00Z"
}
```

Ideal para uso com n8n.