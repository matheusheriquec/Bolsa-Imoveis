# Bolsa Imóveis - Web Scraper OLX

Um web scraper robusto para coletar dados de imóveis da OLX Brasil com suporte a terrenos e propriedades padrão.

## 🎯 Funcionalidades

- **Scraping de Imóveis**: Extrai dados de anúncios de imóveis e terrenos da OLX
- **Suporte a Paginação**: Processa múltiplas páginas automaticamente
- **Detecção de Tipo**: Diferencia automaticamente entre terrenos e imóveis padrão
- **Exportação em Excel**: Salva dados em planilhas formatadas com colunas ajustadas
- **Limpeza de Dados**: Remove caracteres especiais e normaliza preços, áreas e números

## 📋 Requisitos

- Python 3.8+
- Dependências:
  ```bash
  pip install pandas openpyxl beautifulsoup4 curl-cffi
  ```

## 🚀 Como Usar

### Uso Básico (Terrenos em Barra Velha, SC)
```bash
python scraper.py
```

### Com URL Personalizada
```bash
python scraper.py "https://www.olx.com.br/imoveis/apartamentos/estado-sp/sao-paulo"
```

## 📊 Dados Coletados

### Para Terrenos
- Área (m²)
- Tipo de Imóvel
- Preço
- Cidade
- Bairro
- Data de Publicação
- Link do Anúncio

### Para Imóveis Padrão
- Área (m²)
- Tipo de Imóvel
- Preço
- Número de Quartos
- Número de Banheiros
- Vagas de Garagem
- Cidade
- Bairro
- Data de Publicação
- Link do Anúncio

## 🔧 Funcionalidades Técnicas

- **User-Agent Realista**: Simula navegador Chrome para evitar bloqueios
- **Delay Inteligente**: Aguarda 3 segundos entre requisições para respeitar o servidor
- **Tratamento de Erros**: Logs detalhados e recuperação de falhas
- **Limpeza Automática**: Normaliza preços em reais, áreas em m² e números inteiros

## ⚠️ Aviso Legal

Este scraper é fornecido apenas para fins educacionais. Respeite os Termos de Serviço da OLX e a Lei Geral de Proteção de Dados (LGPD).

## 📝 Licença

MIT

## 👨‍💻 Autor

Matheus
