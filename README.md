# ppng-frontend

Interface web do projeto de cálculo da PPNG (Provisão de Prêmios Não Ganhos), desenvolvida como parte do MVP da disciplina de Desenvolvimento Full Stack Básico da PUC-Rio.

Esta aplicação permite que o usuário selecione uma data de fechamento, dispare o cálculo da PPNG via API, visualize o progresso em tempo real e acesse a análise dos resultados.

---

## Funcionalidades

- Seleção da **data base** de fechamento
- Envio da data para a API via `POST`
- Disparo do cálculo da PPNG com exibição de **barra de progresso**
- Redirecionamento automático para a **análise HTML** dos resultados, gerada pela API
- Visual simples, responsivo e agradável

---

## Tecnologias utilizadas

- HTML5
- CSS3 (estilização embutida no HTML)
- JavaScript (Fetch API)

> Não foram utilizados frameworks JS como React, Vue ou Angular, conforme exigência do projeto.

---

## Como executar o front-end

1. Clone este repositório:

```bash
git clone https://github.com/lauragross/ppng-frontend.git
cd ppng-frontend
```

2. Abra o arquivo `index.html` diretamente no navegador (clique duplo ou `Ctrl+O` no navegador):

```
ppng-frontend/index.html
```

> Não é necessário servidor local, extensão, build ou configuração extra. Basta abrir o arquivo no navegador.

---

## Integração com a API

O front-end realiza chamadas às seguintes rotas da API (`ppng-api`):

| Função                    | Rota chamada               |
|---------------------------|----------------------------|
| Definir data base         | `/data_base_fechamento`    |
| Iniciar cálculo da PPNG   | `/calcular_ppng`           |
| Consultar progresso       | `/progresso_ppng`          |
| Visualizar análise        | `/analisar_ppng` (redirect)|

---

## Estrutura do projeto

```
ppng-frontend/
└── index.html  ← página principal (SPA)
```

---

## Desenvolvido por

Laura Gross Lorenzi  
PUC-Rio • MVP - Desenvolvimento Full Stack Básico